# i686-elf-gcc-toolchain

A Docker-powered portable GCC cross compiler for i686-elf, following https://wiki.osdev.org/GCC_Cross-Compiler.

## Installation

Get the prebuilt image via Docker Hub:

```sh
docker pull kevincharm/i686-elf-gcc-toolchain:5.5.0
```

## Usage

Using the compiler:

```sh
docker run --rm kevincharm/i686-elf-gcc-toolchain:5.5.0 bash -c 'i686-elf-gcc --version'
```

GRUB is also available in this image:

```sh
docker run --rm kevincharm/i686-elf-gcc-toolchain:5.5.0 bash -c 'grub-mkrescue --version'
```

## Building from Dockerfile

```sh
docker build -t kevincharm/i686-elf-gcc-toolchain:5.5.0 .
```
