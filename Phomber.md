# Guía de Instalación y Uso de Phomber en Kali Linux

## Descripción
Phomber es una herramienta de OSINT para realizar búsquedas de información de números telefónicos.

## Instalación

Sigue estos pasos para instalar Phomber en Kali Linux:

```bash
# Clonar el repositorio
git clone https://github.com/s41r4j/phomber.git

# Navegar al directorio
cd phomber

# Dar permisos de ejecución a todos los archivos
chmod +x *

# Instalar dependencias (usando --break-system-packages para evitar conflictos)
sudo pip3 install pyproject.toml --break-system-packages
sudo pip3 install mac_vendor_lookup --break-system-packages
```

## Uso

```bash
# Ejecutar la herramienta
sudo python3 phomber.py

# Una vez dentro de la herramienta, usar el comando help para ver las opciones disponibles
help
```

## Ejemplo

```bash
# Buscar información de un número telefónico
number +555555555
```

## Notas importantes
- Es necesario ejecutar con `sudo` para ciertas funcionalidades
- La opción `--break-system-packages` se utiliza para evitar conflictos con paquetes del sistema
- Asegúrate de tener Python3 instalado en tu sistema

## Características
- Búsqueda de información de números telefónicos
- Herramienta de reconnaissance e inteligencia de fuentes abiertas (OSINT)
- Interfaz de línea de comandos intuitiva

## Advertencia
Esta herramienta debe usarse únicamente con fines educativos y de pruebas de penetración autorizadas.
