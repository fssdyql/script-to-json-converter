# script-to-json-converter (LX / Ikun 音源管理助手)

一个基于 PyQt6 开发的桌面端工具，旨在简化 **LX Music (洛雪音乐)** 和 **Ikun Music** 音源脚本（`.js`）的导入、管理与自动更新流程。

[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/framework-PyQt6-green.svg)](https://www.riverbankcomputing.com/software/pyqt/)

## 🚀 核心功能

-   **一键导入**: 支持将多个 `.js` 音源脚本通过拖拽直接导入软件配置。
-   **智能转换**: 自动处理脚本的 Base64 编码与 zlib 压缩（`gz_` 前缀格式），生成兼容的 `user_api.json`。
-   **多版本兼容**: 自动检测并支持 LX Music Desktop 和 Ikun Music Desktop 的数据路径。
-   **Key 提取与更新**: 
    -   自动从现有音源中提取 API Key。
    -   支持通过 Key 联网一键更新音源脚本（兼容 Ikun、聆澜极速/兼容版）。
-   **可视化管理**: 
    -   列表查看已安装音源。
    -   支持拖拽项进行排序。
    -   一键卸载或更新指定音源。
-   **批量导出**: 将软件中已安装的音源一键还原为 `.js` 文件导出到桌面。
-   **隐藏功能**: 内置彩蛋触发机制，支持通过 Key 直接远程下载并安装音源。

## 🛠️ 安装与运行

### 1. 克隆项目
```bash
git clone https://github.com/fssdyql/script-to-json-converter.git
cd script-to-json-converter
```

### 2. 安装依赖
确保你已安装 Python 3.8+，然后安装必要的 GUI 库：
```bash
pip install PyQt6
```

### 3. 运行程序
```bash
python main.py
```

## 📖 使用指南

1.  **导入音源**: 运行程序后，将你的 `.js` 插件文件直接拖入底部的虚线框区域，点击确认即可完成安装。
2.  **管理音源**: 点击“音源管理”，你可以对已安装的插件进行排序（拖动）、删除或单独更新。
3.  **提取 Key**: 如果你安装了带有 Key 的验证版音源，点击“提取已有音源 Key”即可快速备份你的凭据。
4.  **导出备份**: 点击“一键导出现有音源到桌面”，程序会在桌面创建“音源”文件夹，将所有配置还原为 JS 文件。

## ⌨️ 隐藏功能
 通过特定的操作可打开一个彩蛋界面 通过输入 Key 直接从云端获取最新脚本。

## ⚠️ 免责声明
- 本工具仅作为开发者交流学习使用，不提供任何音源脚本。
- 请在遵守相关法律法规的前提下使用，尊重音源作者的版权。
- 因使用第三方插件导致的任何问题与本工具无关。

## 🤝 贡献
欢迎提交 Issue 或 Pull Request 来改进本项目！
