# Preparación de la VM Debian para RamOS

## Especificaciones de la VM
- **Hipervisor**: VirtualBox
- **Sistema Operativo**: Debian GNU/Linux 13.0 "Trixie"
- **Usuario**: ramlinux
- **Arquitectura**: amd64

## Paquetes instalados
```bash
sudo apt install -y build-essential git wget curl gawk bison flex texinfo \
  python3 perl xz-utils bzip2 gzip tar patch libncurses-dev \
  libssl-dev bc rsync kmod cpio
