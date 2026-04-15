<p align="center">
	<img src="logo.png" width="376" height="128" alt="Winlator Logo" />
</p>

# Winlator（中文说明）

Winlator 是一款 Android 应用，可通过 Wine 与 Box86/Box64 运行 Windows（x86_64）应用程序。

## winlator-Next fork 说明

本仓库基于 Winlator 生态进行维护，包含了该代码库中的额外集成工作。

当前仓库结构：
- 主要项目文件位于仓库根目录。
- `app`、`vortek`、`gladio` 为 Git 子模块。

开始本地开发前，请先初始化子模块：

```bash
git submodule update --init --recursive
```

# 安装

1. 在 [GitHub Releases](https://github.com/brunodev85/winlator/releases) 下载并安装 APK（`Winlator_11.0.apk`）
2. 启动应用并等待安装流程完成

----

[![在 Youtube 播放](https://img.youtube.com/vi/ETYDgKz4jBQ/3.jpg)](https://www.youtube.com/watch?v=ETYDgKz4jBQ)
[![在 Youtube 播放](https://img.youtube.com/vi/9E4wnKf2OsI/2.jpg)](https://www.youtube.com/watch?v=9E4wnKf2OsI)
[![在 Youtube 播放](https://img.youtube.com/vi/czEn4uT3Ja8/2.jpg)](https://www.youtube.com/watch?v=czEn4uT3Ja8)
[![在 Youtube 播放](https://img.youtube.com/vi/eD36nxfT_Z0/2.jpg)](https://www.youtube.com/watch?v=eD36nxfT_Z0)

----

# 实用技巧

- 如果遇到性能问题，可在“容器设置 -> 高级”中将 Box64 预设改为 `Performance`。
- 对依赖 .NET Framework 的应用，建议安装“开始菜单 -> 系统工具 -> 安装器”中的 `Wine Mono`。
- 部分老游戏无法启动时，可在“容器设置 -> 环境变量”中添加 `MESA_EXTENSION_MAX_YEAR=2003`。
- 建议通过 Winlator 主屏幕上的游戏快捷方式启动游戏，可为每个游戏单独设置参数。
- 若低分辨率游戏显示异常，可在快捷方式设置中启用 `Force Fullscreen`。
- 为提升 Unity 引擎游戏稳定性，可将 Box64 预设改为 `Stability`，或在快捷方式执行参数中添加 `-force-gfx-direct`。

# 鸣谢与第三方组件

- GLIBC 补丁：[Termux Pacman](https://github.com/termux-pacman/glibc-packages)
- Wine（[winehq.org](https://www.winehq.org/)）
- Box86/Box64：由 [ptitseb](https://github.com/ptitSeb) 提供
- Mesa（Turnip/Zink/VirGL）（[mesa3d.org](https://www.mesa3d.org)）
- DXVK（[github.com/doitsujin/dxvk](https://github.com/doitsujin/dxvk)）
- VKD3D（[gitlab.winehq.org/wine/vkd3d](https://gitlab.winehq.org/wine/vkd3d)）
- CNC DDraw（[github.com/FunkyFr3sh/cnc-ddraw](https://github.com/FunkyFr3sh/cnc-ddraw)）

特别感谢所有参与这些项目的开发者。<br>
感谢所有支持并相信这个项目的人。
