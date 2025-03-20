# NewsFilter 客户端

## 项目介绍

NewsFilter 是一个 macOS 菜单栏应用，帮助用户自动浏览网站并执行内容分析任务。通过简单配置，它可以代替人工操作浏览器，收集和分析网页内容。

本应用基于通义千问视觉模型，能够理解屏幕内容并执行复杂的浏览任务。

## 功能特点

- **智能网页浏览**：AI 助手能自动执行网页浏览操作，包括点击、输入、滚动等
- **内容分析**：可以分析网页内容，提取关键信息，生成摘要
- **便捷菜单栏访问**：常驻 macOS 菜单栏，随时可用
- **自定义指令**：支持创建和保存个性化的任务指令
- **多网站管理**：可添加多个目标网站并快速切换
- **状态通知**：直观显示任务执行状态，完成后发送系统通知

## 应用演示

![image](https://github.com/WhereAreMySOCKS/NewsFilter-client/blob/main/demo/demo.gif)

## 使用方法

### 快速开始

1. 启动应用后，首先配置 API 密钥（设置→配置API Key）
2. 添加一个网站（我的网站→添加）
3. 创建一个指令（我的指令→添加）
4. 选择网站和指令，点击"开始任务"


### 保存常用配置

1. 选择一个网站和一个指令
2. 点击"保存当前配置"
3. 之后可以在"我的配置"菜单中快速选择此组合

## 实用提示

- **指令设计**：写清晰具体的指令可以获得更好的执行效果
- **任务监控**：任务执行过程中可以查看浏览器窗口了解进度
- **使用本地浏览器**：应用会使用您的Chrome浏览器，保留已有的登录状态
- **查看日志**：如遇问题，可通过"设置→查看日志"了解详情

## 应用打包

如需将应用打包为独立程序：

```bash
pip install pyinstaller
pyinstaller --windowed --name "NewsFilter" --icon=icon/idle_icon.png menubar_app.py
```

打包后的应用可直接拖入应用程序文件夹使用。

## 系统要求

- macOS 10.14 或更高版本
- Python 3.8+
- Chrome 浏览器（推荐）
- 通义千问API密钥

## 技术简介

NewsFilter 使用 Playwright 实现浏览器自动化，通过视觉AI模型理解屏幕内容并做出决策。应用界面采用原生 macOS 风格设计，提供良好的用户体验。

---

*注：本项目会持续优化功能和性能，欢迎提供使用反馈。* 