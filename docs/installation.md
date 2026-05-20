# 📖 安装指南

本文档介绍如何安装和配置 PM AI Skills。

## 前置要求

在开始之前，请确保你已经：

- ✅ 安装了 [Claude Code](https://claude.ai/code)
- ✅ 熟悉基本的 AI Skills 使用方式
- ✅ 有基本的命令行操作经验

## 安装步骤

### 1. 克隆仓库

```bash
git clone https://github.com/Yoyogithup/pm-ai-skills.git
cd pm-ai-skills
```

### 2. 浏览可用技能

查看 `skills/` 目录下的各个分类：

```bash
ls -la skills/
```

你会看到以下分类：
- `product-work/` - 产品工作相关技能
- `daily-life/` - 日常生活相关技能  
- `project-management/` - 项目管理相关技能
- `fun-skills/` - 有趣的创意技能

### 3. 选择需要的技能

进入你感兴趣的技能目录，查看 README 了解详情：

```bash
cd skills/product-work/prd-doc-writer/
cat README.md
```

### 4. 安装技能到 Claude Code

根据 Claude Code 的 skills 安装方式：

**方式 1：直接复制文件**
将 `skill.md` 复制到 Claude Code 的 skills 目录

**方式 2：符号链接**（推荐）
```bash
ln -s /path/to/pm-ai-skills/skills/product-work/prd-doc-writer/skill.md \
      ~/.claude/skills/prd-doc-writer.md
```

### 5. 验证安装

在 Claude Code 中输入技能名称（如 `/prd-doc-writer`），看是否能正常调用。

## 常见问题

### Q: 技能无法加载？
A: 检查文件路径是否正确，确保 `skill.md` 文件存在且格式正确。

### Q: 如何更新技能？
A: 使用 `git pull` 拉取最新代码，如果使用符号链接，会自动更新。

### Q: 可以同时安装多个技能吗？
A: 可以！每个技能是独立的，互不影响。

## 下一步

- 📘 查看 [使用指南](./usage-guide.md) 学习如何使用技能
- 📙 查看 [开发指南](./development.md) 学习如何创建自己的技能

---

如有问题，欢迎提 [Issue](https://github.com/Yoyogithup/pm-ai-skills/issues)！
