# 欢迎使用你的 VS Code 插件

## 文件夹内容

- 此文件夹包含插件所需的所有文件。
- `package.json` - 这是清单文件，用于声明插件和命令。
  - 示例插件注册了一个命令并定义了其标题和命令名称。有了这些信息，VS Code 就可以在命令面板中显示该命令，此时还不需要加载插件。
- `src/extension.ts` - 这是主文件，你将在此提供命令的实现。
  - 该文件导出一个 `activate` 函数，在插件首次激活时调用（本例中是通过执行命令激活）。在 `activate` 函数内部，我们调用 `registerCommand`。
  - 我们将包含命令实现的函数作为第二个参数传递给 `registerCommand`。

## 快速开始

- 按 `F5` 打开一个加载了你插件的新窗口。
- 按 `Ctrl+Shift+P`（Mac 上为 `Cmd+Shift+P`）打开命令面板，输入 `Hello World` 来运行你的命令。
- 在 `src/extension.ts` 中设置断点来调试你的插件。
- 在调试控制台中查看插件的输出。

## 修改代码

- 修改 `src/extension.ts` 中的代码后，可以从调试工具栏重新启动插件。
- 也可以重新加载（`Ctrl+R` 或 Mac 上的 `Cmd+R`）VS Code 窗口来加载你的更改。

## 探索 API

- 打开 `node_modules/@types/vscode/index.d.ts` 文件可以查看完整的 API 集。

## 运行测试

- 安装 [Extension Test Runner](https://marketplace.visualstudio.com/items?itemName=ms-vscode.extension-test-runner)
- 通过 **Tasks: Run Task** 命令运行 "watch" 任务。确保它正在运行，否则可能无法发现测试。
- 从活动栏打开测试视图，点击 "Run Test" 按钮，或使用快捷键 `Ctrl/Cmd + ; A`
- 在测试结果视图中查看测试结果输出。
- 修改 `src/test/extension.test.ts` 或在 `test` 文件夹中创建新的测试文件。
  - 提供的测试运行器只会考虑匹配 `**.test.ts` 命名模式的文件。
  - 你可以在 `test` 文件夹中创建子文件夹，以任何方式组织你的测试。

## 进阶

- [遵循 UX 指南](https://code.visualstudio.com/api/ux-guidelines/overview) 创建与 VS Code 原生界面和模式无缝集成的插件。
- 通过[打包插件](https://code.visualstudio.com/api/working-with-extensions/bundling-extension)减小插件大小并提高启动速度。
- 在 VS Code 插件市场上[发布你的插件](https://code.visualstudio.com/api/working-with-extensions/publishing-extension)。
- 通过设置[持续集成](https://code.visualstudio.com/api/working-with-extensions/continuous-integration)自动化构建。
- 集成[问题报告](https://code.visualstudio.com/api/get-started/wrapping-up#issue-reporting)流程，让用户报告问题和功能请求。

## 开发与构建

### 安装依赖

首次开发需要安装 `@vscode/vsce` 工具：

```bash
pnpm add -D @vscode/vsce
```

### 可用命令

```bash
# 编译插件
pnpm run build

# 打包插件（生成 .vsix 文件到 dist 目录）
pnpm run package

# 发布插件到市场
pnpm run publish

# 监听文件变化并自动编译
pnpm run watch

# 运行代码检查
pnpm run lint

# 运行测试
pnpm run test

# 删除发布者
npx vsce delete-publisher publisher-id
```
