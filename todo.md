多种内核模型（包括新旧I/A处理器，KVM/openVZ/docker等，预留3系列，4系列LTS内核供无法兼容新内核的设备）

调试OpenRC，实在不行继续用systemd

确认python3与python2软件的代码问题，准备好patch，方便默认py迁移至py3

设计命令行版简化版安装程序

确认默认vim/nano/emacs/ne风格，设计一个迷你的包管理器，只负责给用户安装配置文件

尽快确认徽标，主题颜色

ARM版确认将提供，但不确认是否armhf, aarch64，ARM版讲提供strong和lite两种版本，strong版为glibc，不压缩不裁剪，lite版使用musl，内核裁剪，默认软件压缩

如果MIPS架构和SHENWEI(申威)架构需要定当移植。
