# tool-kit

**tool-kit** 是一个为开发者和运维工程师精心挑选的 VS Code 扩展包 (Extension Pack)。它集成了日常开发 (Golang, Frontend) 和 DevOps (Terraform, Cloud) 工作流中必不可少的工具，旨在帮助团队统一开发环境，提高工作效率。

## 包含的扩展

安装此扩展包将自动安装以下工具：

### 🛠️ 语言与框架支持

- **Go** (`golang.go`): 官方 Go 语言支持，提供智能感知、调试等功能。
- **Terraform** (`hashicorp.terraform`): HashiCorp 官方 Terraform 支持。
- **HCL** (`hashicorp.hcl`): HCL 语言高亮与语法支持。
- **YAML** (`redhat.vscode-yaml`): 全面的 YAML 语言支持。
- **Protobuf** (`drblury.protobuf-vsc`): Protocol Buffers 语法高亮。
- **SaltStack** (`korekontrol.saltstack`): SaltStack 语法高亮与代码片段。

### 🚀 生产力与代码质量

- **Prettier** (`esbenp.prettier-vscode`): 固执己见的代码格式化工具。
- **Oxc** (`oxc.oxc-vscode`): 高性能的 JavaScript/TypeScript 工具链。
- **Vim** (`vscodevim.vim`): 为 VS Code 提供 Vim 模拟。
- **Project Manager** (`alefragnani.project-manager`): 轻松切换与管理多个项目。

### 🌳 Git 与版本控制

- **GitLens** (`eamodio.gitlens`): 增强 VS Code 内置的 Git 功能。
- **Git Graph** (`mhutchie.git-graph`): 查看 Git 提交历史的图形化界面。
- **GitHub Local Actions** (`sanjulaganepola.github-local-actions`): 在本地运行 GitHub Actions。

### ☁️ 远程开发与运维

- **Remote - SSH** (`ms-vscode-remote.remote-ssh`): 通过 SSH 连接到远程服务器进行开发。
- **Remote Explorer** (`ms-vscode.remote-explorer`): 远程资源管理器。
- **SOPS** (`signageos.signageos-vscode-sops`): 编辑 SOPS 加密文件。

## 使用说明

安装本扩展包后，上述所有扩展将作为依赖项自动安装。如果想要卸载某个特定扩展，可以单独禁用或卸载它，但建议保留以获得最佳体验。

## 配置

本扩展包本身无需额外配置。各个子扩展的配置（如 `go.gopath`, `prettier.printWidth` 等）请参考各自的官方文档进行设置。

## 贡献

欢迎通过 Issue 提交反馈或建议添加新的实用扩展。

## 许可证

MIT License
