# 变更日志
本文件记录 "tool-kit" 插件的所有重要变更。
参考 [Keep a Changelog](http://keepachangelog.com/) 了解如何组织此文件。

## [1.2.0] - 2026-02-10

### 新增
- 添加环境配置示例文件 `.env.example`
- 添加 OVSX 市场发布支持

### 修复
- 降低 VS Code 引擎版本要求至 `^1.95.0`，以兼容 Antigravity 和 Kiro

### 优化
- 优化发布流程，支持同时发布到 VS Code Marketplace 和 Open VSX Registry
- 更新发布工具依赖（`dotenv-cli`、`ovsx`）
- 改进 `.gitignore` 和 `.vscodeignore` 配置
- 优化快速启动文档内容

## [1.1.0] - 2026-02-10

### 新增
- 添加 `build` 编译脚本,用于构建插件
- 添加 `package` 脚本,用于打包插件为 .vsix 文件
- 添加 `publish` 脚本,用于发布插件到市场

## [1.0.0] - 初始版本

- 初始版本发布
