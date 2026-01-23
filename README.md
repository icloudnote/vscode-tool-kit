# devops-kit

devops-kit 是一个帮助开发者与运维团队提高日常工作效率的 VS Code 扩展集合。它提供若干实用的命令与工具，用于常见的 DevOps 任务自动化与快速导航。

## 主要功能

- 快速执行常用 DevOps 命令（示例：构建、打包、查看日志）。
- 在工作区内快速跳转到 DevOps 相关文件与脚本。
- 提供可配置的任务模板与提示，方便在 CI/CD 中复用。

## 安装

- 从源码安装（开发）：
  1.  安装依赖：`pnpm install` 或 `npm install`
  2.  编译：`pnpm run compile` 或 `npm run compile`
  3.  在 VS Code 中按 `F5` 启动扩展调试窗口

- 打包为 VSIX：
  1.  确保编辑并保存了本项目的 `README.md`（本文件）
  2.  运行：`vsce package`

## 使用示例

- 在命令面板（`Cmd+Shift+P`）中输入 `Devops: ` 可查看本扩展提供的所有命令。
- 常见命令：
  - `Devops: Run Build` — 在当前工作区触发构建脚本。
  - `Devops: Open Logs` — 打开常用日志文件或日志目录。

（注：具体命令以 `package.json` 中的 `contributes.commands` 为准。）

## 配置

如有扩展设置，会在 `package.json` 的 `contributes.configuration` 中声明。常见配置项示例：

- `devopsKit.defaultShell`：指定运行脚本时使用的 shell（默认 `/bin/zsh`）。
- `devopsKit.logPaths`：日志路径数组，用于 `Open Logs` 命令。

## 贡献

欢迎提交 Issue 或 PR。贡献前请先阅读贡献指南并确保代码风格一致。

## 许可证

本项目遵循 MIT 许可证，详见 LICENSE 文件。
