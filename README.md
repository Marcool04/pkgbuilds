# fwcd's Arch Repository

[![Build](https://github.com/fwcd/arch-repo/actions/workflows/build.yml/badge.svg)](https://github.com/fwcd/arch-repo/actions/workflows/build.yml)

An [unofficial package repository](https://wiki.archlinux.org/title/unofficial_user_repositories) for Arch Linux (`pacman`), mainly sourced from the [AUR](https://aur.archlinux.org). Binaries are built and deployed for the following architectures:

| Architecture | Build |
| ------------ | ----- |
| [x86_64](https://github.com/fwcd/arch-repo-x86_64) | [![Build](https://github.com/fwcd/arch-repo-x86_64/actions/workflows/build.yml/badge.svg)](https://github.com/fwcd/arch-repo-x86_64/actions/workflows/build.yml) |
| [aarch64](https://github.com/fwcd/arch-repo-aarch64) | [![Build](https://github.com/fwcd/arch-repo-aarch64/actions/workflows/build.yml/badge.svg)](https://github.com/fwcd/arch-repo-aarch64/actions/workflows/build.yml) |

## Usage

Add the following to your `/etc/pacman.conf`:

```
[fwcd]
Server = https://github.com/fwcd/arch-repo-$arch/releases/latest/download
SigLevel = Never
```

## See also

- [`archlinuxarm-images`](https://github.com/fwcd/archlinuxarm-images.git) (Unofficial prepartitioned images of Arch Linux ARM)
- [`archlinuxarm-docker`](https://github.com/fwcd/archlinuxarm-docker.git) (Unofficial Docker images of Arch Linux ARM)
