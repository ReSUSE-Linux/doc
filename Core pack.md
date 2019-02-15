## `SPEC`打包规范 ( 第一版 )
> 1. 不要在开头增加项目注释说明，后期统一添加；
> 2. 不是肯定下来需要添加的 `patch` 不要添加 (`openSUSE` 的`patch`较多，注意剥离)；
> 3. 打包从简，不是必须拆的包不拆包；
> 4. 少留空档，暂时不写 `Changelog` `Dependency`；
> 5. 只打包 `amd64` 架构，暂时不打包其他架构 (含`i586`) ；

## **`core` 包** ( 参考 `Arch Linux` ）

### `Core` 库
| 软件包          | 软件包          | 软件包         | 软件包        | 软件包           |
| --------------- | --------------- | -------------- | ------------- | ---------------- |
| `bash`          | ~~`bzip2`~~     | `coreutils`    | `cryptsetup`  | `device-mapper`  |
| `dhcpcd`        | `e2fsprogs`     | `file`         | `filesystem`  | `findutils`      |
| `gawk`          | `gcc-libs`      | `gettext`      | `grep`        | `inetutils`      |
| `iproute2`      | `iputils`       | `jfsutils`     | `linux`       | `linux-firmware` |
| `logrotate`     | `lvm2`          | `man-db`       | `man-pages`   | `mdadm`          |
| `netctl`        | `pciutils`      | `perl`         | `procps-ng`   | `psmisc`         |
| `reiserfsprogs` | `s-nail`        | `sed`          | `shadow`      | `sysfsutils`     |
| `texinfo`       | `usbutils`      | `util-linux`   | `which`       | `xfsprogs`       |
| `autoconf`      | `automake`      | `binutils`     | `bison`       | `fakeroot`       |
| `file`          | `findutils`     | `flex`         | `gawk`        | `gettext`        |
| `which`         | `groff`         | `m4`           | `make`        | `patch`          |
| `pkgconf`       | `sed`           | `sudo`         | `texinfo`     | `util-linux`     |
| `(!) gcc`       | `(+) pacman`    | `(+) ruby`     | `(+) zipper`  | `(+) libzypp`    |
| ~~`less`~~      | ~~`diffutils`~~ | ~~`gzip`~~     | ~~`libtool`~~ | ~~`tar`~~        |
| ~~`nano`~~      | ~~`(?) xz`~~    | ~~`(?) gdbm`~~ | `(?)licenses` | `(?) yast`       |
| `(?)vi`         |                 |                |               |                  |

> * `(+)` 为非 `core` 库，但被 `zypper` 需要，`(!)` 为优先打包项目，删除线为已完成打包项目，`(?)` 为待定打包项目；
> * 不打 `systemd` 相关包 `systemd`， `systemd-sysvcompat`， `systemd-sysvcompat`；
> * 当前已打不在`core`库的包：`neofetch`

## 当前打包任务部署

| 打包者                | 当前任务 | 当前任务 | 当前任务 |
| --------------------- | -------- | -------- | -------- |
| `Zypper`              | `bzip2`  |          |          |
| `OBS`                 | `grep`   |          |          |
| `openSUSE-TumbleWeed` | `sed`    |          |          |
| `Yast`                | `glibc`  |          |          |
