# Glibc - Pass 1

## Información del paquete
- **Nombre**: Glibc
- **Versión**: 2.40
- **Fuente**: https://ftp.gnu.org/gnu/glibc/glibc-2.40.tar.xz

## Dependencias
- GCC Pass 1
- Binutils Pass 1
- Kernel headers 6.1.0

## Configuración
```bash
../glibc-2.40/configure \
    --prefix=$LFS/tools \
    --host=$LFS_TGT \
    --build=$(../glibc-2.40/scripts/config.guess) \
    --enable-kernel=4.19 \
    --with-headers=$LFS/usr/include \
    --disable-nscd \
    libc_cv_slibdir=$LFS/tools/lib
