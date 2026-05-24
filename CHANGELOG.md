# 更新日志 / Changelog

本项目遵循[语义化版本](https://semver.org/lang/zh-CN/)。版本号即桌面端安装包版本。
This project adheres to [Semantic Versioning](https://semver.org/). The version number is the desktop installer version.

## [0.1.2] - 2026-05-24

### 变更 / Changed
- 统一品牌显示名为 **Reel Video**（此前桌面端、安装包、窗口标题等处混用 “Real Video”）。安装包文件名相应变为 `Reel Video_0.1.2_x64-setup.exe`。`identifier`（`com.reel.video`）保持不变，用户数据目录不受影响。
  Unified the display name to **Reel Video** (the desktop app, installer, and window title previously showed “Real Video” inconsistently). The installer is now `Reel Video_0.1.2_x64-setup.exe`. The `identifier` (`com.reel.video`) is unchanged, so user data directories are preserved.

### 优化 / Improved
- 全局滚动条改为纤细、半透明、圆角样式，悬停时才加深，替换 WebView2 默认的粗滚动条（在生成视频页右侧尤其明显）。
  Slimmer, semi-transparent, rounded scrollbars that darken only on hover, replacing the chunky default WebView2 bar (most noticeable on the Generate Video page).

### 文档 / Docs
- README 具名标注上游来源（fork 自 AIDC-AI 的 [Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video)），新增「相对上游的改动」小节与「本地优先」说明。
  README now explicitly attributes the upstream source (a fork of AIDC-AI’s [Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video)), with a “Changes from upstream” section and a “local-first” note.

## [0.1.1] - 2026-05-24

### 新增 / Added
- 桌面端中英文界面切换（i18n）。
  Chinese / English UI switching (i18n) for the desktop app.

## [0.1.0] - 2026-05-24

### 新增 / Added
- 首个桌面端版本：基于 Tauri 2.0 的跨平台外壳，安装包内置 FastAPI 后端（sidecar），下载即用；移除原 Streamlit Web UI 与 Docker 部署方式。
  First desktop release: a cross-platform Tauri 2.0 shell with the FastAPI backend bundled as a sidecar (download-and-run); removed the original Streamlit web UI and Docker deployment.
