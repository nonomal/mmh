# 简介

mmh 创立之初只是为了快速的链接到跳板机之后的目标机器，随着不断的完善目前已经具备了以下能力:

- 无限的跳板机自动穿透(`A -> B -> C -> ... -> Target Server`)
- 在无限跳板功能基础上实现远程命令执行，且支持管道式操作(允许执行 `tail -f` 类似的命令)
- 在远程命令执行基础上增强的批量执行，并为多台服务器日志添加不同颜色的日志前缀(颜色顺次滚动)
- 基于无限跳板的跨跳板机文件/目录上传与下载(不支持服务端多文件下载到本地)，且支持批量化上传
- 基于无限跳板的远端 ping 检测，例如跳板链路 `A -> B -> C`，A 可以直接 ping C 来检测 C 状态
- 基于无限跳板的 tun 打洞，且支持反转(本地监听 -> 远端端口 or 远端监听 -> 本地端口)

在这些主要功能的基础上也增加了一些比较人性化的功能，比如多配置文件切换、配置文件层级覆盖、跳板机穿越次数的安全检测等。

[Quick Start](quick_start) 包含了 mmh 的快速开始文档，你可以直接根据文档进行快速体验。

[首页](.) | [下一页](quick_start)