## **`core` 包** ( 参考 [`Arch Linux`](https://www.archlinux.org/packages/ "Arch Linux Packages") ）

### `Core` 库
| 软件包           | 软件包           | 软件包          | 软件包         | 软件包           |
| --------------- | --------------- | -------------- | ------------- | ---------------- |
| `bash`          | ~~`bzip2`~~     | `coreutils`    | `cryptsetup`  | `device-mapper`  |
| `dhcpcd`        | `e2fsprogs`     | `file`         | `filesystem`  | `findutils`      |
| `gawk`          | `gcc-libs`      | `gettext`      | `grep`        | `inetutils`      |
| `iproute2`      | `iputils`       | `jfsutils`     | `linux`       | `linux-firmware` |
| `logrotate`     | `lvm2`          | `man-db`       | `man-pages`   | `mdadm`          |
| `netctl`        | `pciutils`      | `perl`         | `procps-ng`   | `psmisc`         |
| `reiserfsprogs` | `s-nail`        | `sed`          | `shadow`      | `sysfsutils`     |
| `texinfo`       | `usbutils`      | `util-linux`   | `which`       | `xfsprogs`       |
| `autoconf`      | `automake`      | `(!)binutils`  | `bison`       | `fakeroot`       |
| `file`          | `findutils`     | `flex`         | `gawk`        | `gettext`        |
| `which`         | `groff`         | `m4`           | `make`        | `patch`          |
| `pkgconf`       | `sed`           | `sudo`         | `texinfo`     | `util-linux`     |
| `(!) gcc`       | `(+) ruby`      | `(+) zypper`   | `(+) libzypp` | ~~`nano`~~       |
| ~~`less`~~      | ~~`diffutils`~~ | ~~`gzip`~~     | ~~`libtool`~~ | ~~`tar`~~        |
| `(?)vi`         | ~~`(?) xz`~~    | ~~`(?) gdbm`~~ | `(?)licenses` | `(?) yast`       |

> * `(+)` 为非 `core` 库，但被 `zypper` 需要，`(!)` 为优先打包项目，删除线为已完成打包项目  
>   `(?)` 为待定打包项目
> * 不打 `systemd` 相关包 `systemd` `systemd-sysvcompat` `systemd-sysvcompat` `pacman`
> * 当前已打不在`core`库的包：`neofetch`

## 当前打包任务部署

| ReSUSEr               | 开发维护    | 开发维护        | 开发维护     | 开发维护  |
| --------------------- | ---------- | -------------- | ------------| -------- |
| `Zypper`              | `e2fsprogs`| `file`         | `findutils` |          |
| `OBS`                 | `grep`     |                |             |          |
| `openSUSE-TumbleWeed` | `sed`      |                |             |          |
| `Yast`                | `glibc`    | `core_pack.md` |             |          |

## 常用资源链接
* [`Arch Linux Core Repo`](https://www.archlinux.org/packages/?repo=Core "Arch Linux Core Repo Search")  [`Arch Linux base Group`](https://www.archlinux.org/groups/x86_64/base/ "Arch Linux base Group")  [`Arch Linux base-devel Group`](https://www.archlinux.org/groups/x86_64/base-devel/ "Arch Linux base-devel Group")  [`ArchLinux AUR`](https://aur.archlinux.org/ "The Arch Linux User-community Repository")
* [`Fedora Rawhide SPECs`](https://dl.fedoraproject.org/pub/fedora/linux/development/rawhide/Workstation/source/tree/Packages/ "Fedora Rawhide SPECS")
* [`openSUSE Tumbleweed SPECs`](http://opensuse.mirror.liquidtelecom.com/source/tumbleweed/repo/ "风滚草的SPEC")
* [`RPM Packaging Guide`](https://rpm-packaging-guide.github.io/ "RPM 打包手册")
* [`LFS v8.3`](http://www.linuxfromscratch.org/lfs/view/stable/ "The LFS Stable Book")  [`BLFS 8.3`](http://www.linuxfromscratch.org/blfs/view/stable/ "The BLFS Stable Book")
