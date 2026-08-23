# musl-cross

This is a simple, lightweight project for making cross-compilation toolchain with musl libc.

## Supported targets

| Target                         | Kernel  | Binutils | GCC    | Musl   | Mold |
|--------------------------------|---------|----------|--------|--------|------|
| aarch64-unknown-linux-musl     | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| arm-unknown-linux-musleabi     | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| arm-unknown-linux-musleabihf   | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| armv7-unknown-linux-musleabi   | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| armv7-unknown-linux-musleabihf | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| i586-unknown-linux-musl        | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| i686-unknown-linux-musl        | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| loongarch64-unknown-linux-musl | 5.19.16 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| m68k-unknown-linux-musl        | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| microblazeel-xilinx-linux-musl | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| microblaze-xilinx-linux-musl   | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| mipsel-unknown-linux-musl      | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| mipsel-unknown-linux-muslsf    | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| mips-unknown-linux-musl        | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| mips-unknown-linux-muslsf      | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| mips64el-unknown-linux-musl    | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| mips64-unknown-linux-musl      | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| or1k-unknown-linux-musl        | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | N/A  |
| powerpcle-unknown-linux-musl   | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| powerpc-unknown-linux-musl     | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| powerpc64le-unknown-linux-musl | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| powerpc64-unknown-linux-musl   | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| riscv32-unknown-linux-musl     | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| riscv64-unknown-linux-musl     | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| s390x-ibm-linux-musl           | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| sh4-multilib-linux-musl        | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |
| x86_64-unknown-linux-musl      | 5.4.296 | 2.47     | 16.2.0 | 1.2.6  | 2.41 |

## How to use

Download the tarball from the [release page](https://github.com/cross-tools/musl-cross/releases) and extract it to `/opt/x-tools`:

```sh
sudo mkdir -p /opt/x-tools
sudo tar -xf ${target}.tar.xz -C /opt/x-tools
```

## How to build

Fork this project and create a new release, or build manually:

```sh
./scripts/make ${target}
```

## License

MIT

## Acknowledgements

We would like to express our gratitude to the following individuals and projects:

- [crosstool-ng](https://github.com/crosstool-ng/crosstool-ng)
- [musl-libc](https://musl.libc.org)
