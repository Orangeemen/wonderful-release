# 🐙 Wonderfor GitHub Release Mirrors

<div align="center">
  <img src="https://mirrors.sdu.edu.cn/assets/logo_big-Dn2qexAM.png" 
       alt="Wonderfor Mirror Logo" 
       width="256" 
       style="border-radius: 16px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" />
</div>

这个仓库存放优秀 GitHub 仓库的列表，以便镜像站定期下载这些仓库的最新的 GitHub Release。你也可以在这里提出新的GitHub Release镜像申请或进行相关讨论。

仓库列表点击 [这里](./repos.yaml) 打开。镜像站在 [这里](https://mirrors.sdu.edu.cn/github-release/) 缓存了这些安装包。
---

## 快速开始

### 提交新的GitHub Release镜像申请
1. **搜索现有Issues**：确认您的申请未重复提交
2. **阅读行为与收录规则**：[POLICY.md](./POLICY.md)
2. **新建 Issue**：选择模板 `GitHub Release镜像申请`
3. **填写完整信息**：帮助维护者高效评估

### 通用软件源同步申请、BUG反馈等其他事项  
> 此类申请请前往主仓库 👉 [🔗 Issues](https://github.com/SDU-Mirrors/issues)


---

## 📝 申请前自查清单

提交前请逐项核对，以便于我们更好的评估

```markdown
- [ ] 项目为 Public 仓库且包含明确 LICENSE 文件
- [ ] Release 页面包含可分发的二进制/安装包资产
- [ ] 项目有持续维护记录（非归档/废弃状态）

🎯 偏好自评（非强制，但显著影响优先级）
- [ ] 属于「小而美」类型（功能聚焦 / 体积轻量 / 构建透明）
- [ ] 非 Electron 应用，或已说明需镜像 Electron 项目的具体理由
- [ ] Release 资产**不捆绑运行时**
- [ ] 已明确实际需要的架构/格式子集（避免全量枚举）
- [ ] installer 与 portable 版内容差异显著，或已指定仅需其一

📦 存储评估
- [ ] 单个项目预估存储合理
- [ ] 已检查不存在国内官方可用分发源