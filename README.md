# Wonderfor GitHub Release Mirrors

<div align="center">
  <img src="https://mirrors.sdu.edu.cn/assets/logo_big-Dn2qexAM.png" 
       alt="Wonderfor Mirror Logo" 
       width="256" 
       style="border-radius: 16px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" />
</div>

这个仓库存放优秀 GitHub 仓库的列表，以便镜像站定期下载这些仓库的最新的 GitHub Release。你也可以在这里提出新的GitHub Release镜像申请或进行相关讨论。

### 仓库列表点击 [这里](./repos.yaml) 打开。镜像站在 [这里](https://mirrors.sdu.edu.cn/github-release/) 缓存了这些安装包。

---

## 快速开始

### 提交新的GitHub Release镜像申请
1. **搜索现有Issues**：确认您的申请未重复提交
2. **阅读行为与收录规则**：[POLICY.md](./POLICY.md)
2. **新建 Issue**：选择模板 `GitHub Release镜像申请`
3. **填写完整信息**：帮助维护者高效评估

👉 [🔗 点击此处提交新申请](../../issues/new/choose)

### 通用软件源同步申请、BUG反馈等其他事项  
> 此类申请请前往主仓库 👉 [SDU-Mirrors/issues](https://github.com/SDU-Mirrors/issues)

---

## 📝 申请前自查清单

提交前请逐项核对，以便于我们更好的评估

```markdown
- [ ] 项目为 Public 仓库且包含明确 LICENSE 文件
- [ ] Release 页面包含可分发的二进制/安装包资产
- [ ] 项目有持续维护记录（非归档/废弃状态）

 项目评估（非强制，但显著影响优先级）
- [ ] 属于「小而美」类型（功能聚焦 / 体积轻量 / 构建透明）
- [ ] 非 Electron 应用，或已说明需镜像 Electron 项目的具体理由
- [ ] Release 资产**不捆绑运行时**，或仅需同步不含运行时的文件
- [ ] 已明确实际需要的架构/格式子集（避免全量枚举）
- [ ] installer 与 portable 版内容差异显著，或已指定仅需其一

 存储评估
- [ ] 单个项目预估存储合理
- [ ] 已检查不存在国内官方可用分发源

## GitHub Release 收录细则

为了合理利用镜像站的存储与带宽资源，确保持续、稳定地为开发者提供服务，我们对申请收录的开源项目制定了以下偏好与底线规则：

### 1. 基本原则与收录偏好

1. 合法合规与开源：项目不得包含违规内容，必须基于公认的开源协议且允许再分发。
2. 推崇“小而美”：我们偏好于那些体积小巧、功能聚焦、代码精简的优秀开源项目。
3. 偏好轻量级应用：倾向于收录非 Electron 架构的项目；倾向于收录不自带庞大运行时（Runtime）的产物（例如：依赖系统已安装框架的 C# / .NET 程序，而非自包含（Self-contained）的巨无霸包）

### 将会慎重考虑收录的情况

1. 臃肿的发行版：如果该项目的 Release 默认打包了整个运行环境（如 Electron），本站将谨慎收录或直接拒绝该类产物的全量镜像申请。
2. 交叉编译的枚举泛滥：对于在 Release 中枚举列出数十种不同架构（如 x86, x64, arm, arm64, mips64, riscv64 等各个系统组合）的项目，我们原则上只收录主流平台（如 Win/Mac/Linux 的 x64/arm64 核心产物），不收录全量文件，申请者需在 Issue 中明确指出需要加速的 1~3 个核心基础文件。
3. 高度重复的产物：如果项目的 Release 同时且大量提供 Installer（安装版）和 Portable（便携版/绿色版），且内容高度重复，本站将拒绝全量收录，申请者需明确指出需要加速的少数核心基础文件。

[行为与收录规则](./POLICY.md)