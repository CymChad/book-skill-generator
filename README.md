# Book Skill Generator

<div align="center">

📚 **从书籍中提取核心方法论，生成可执行的 AI Skill**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![OpenClaw](https://img.shields.io/badge/Platform-OpenClaw-blue)](https://openclaw.ai)
[![Claude Code](https://img.shields.io/badge/Platform-Claude_Code-orange)](https://claude.ai)

**支持 OpenClaw、Claude Code 等主流 AI 应用**

</div>

---

从书籍中提取核心方法论，为每个方法论生成一个独立的、可安装的 AI Skill。支持多个主流 AI 平台使用。

## 功能特点

- **自动提取方法论:** 通过网络搜索，自动提取书籍的核心方法论
- **生成独立 skill:** 为每个方法论生成一个独立的、可安装的 skill 文件
- **完整结构:** 每个 skill 包含完整的适用场景、执行步骤、输出格式等
- **易于使用:** 生成的 skill 可通过斜杠命令直接调用
- **跨平台兼容:** 支持 OpenClaw、Claude Code 等多个主流 AI 应用

## 为什么选择 Book Skill Generator？

### 🌍 跨平台支持
- **一处编写，多处使用** - 生成的 Skill 可在多个 AI 平台使用
- **标准格式** - 遵循通用的 Skill 规范，确保兼容性
- **灵活安装** - 支持口语化安装或手动安装

### 📚 知识转化
- **从阅读到实践** - 将书籍知识转化为可执行的工具
- **系统化方法论** - 每个方法论都有清晰的步骤和输出格式
- **持续积累** - 可以不断为更多书籍生成 Skill

### 🎯 实用导向
- **真实案例** - 每个方法论都包含经典案例和示例
- **即插即用** - 安装后立即可用，无需额外配置
- **可定制** - 可根据实际需求调整和优化

## 平台兼容性

本 Skill 支持以下主流 AI 应用平台：

| 平台 | 安装方式 | 状态 |
|------|---------|------|
| **OpenClaw** | 口语化安装（推荐） | ✅ 完全支持 |
| **Claude Code** | 手动复制到 `.claude/skills/` | ✅ 完全支持 |
| **其他平台** | 手动安装 | ✅ 兼容标准格式 |

## 安装方法

### OpenClaw（推荐）

**方式 1: 口语化安装（最简单）**

在 OpenClaw 中直接说：

```
帮我安装下 https://github.com/CymChad/book-skill-generator
```

或

```
安装这个 skill：https://github.com/CymChad/book-skill-generator
```

OpenClaw 会自动帮你安装！

**方式 2: 命令行安装**

```bash
npx skills add https://github.com/CymChad/book-skill-generator
```

或使用 Git 地址：

```bash
npx skills add git@github.com:CymChad/book-skill-generator.git
```

### Claude Code

手动安装到 Claude Code skills 目录：

```bash
# 克隆仓库
git clone https://github.com/CymChad/book-skill-generator.git

# 复制到 Claude Code skills 目录
mkdir -p ~/.claude/skills/
cp -r book-skill-generator ~/.claude/skills/
```

### 其他平台

对于其他支持 Skill/Plugin 机制的 AI 应用：

1. 克隆仓库：
```bash
git clone https://github.com/CymChad/book-skill-generator.git
```

2. 根据平台要求，将 `SKILL.md` 文件复制到对应的 skills/plugins 目录

## 使用方法

### 1. 调用 Skill

在支持的 AI 应用中输入：

```
从《书籍名称》提取方法论，生成对应的 skill
```

或

```
把《书籍名称》的方法论变成 skill
```

**示例：**
- "从《精益创业》提取方法论，生成对应的 skill"
- "把《原子习惯》的方法论变成 skill"
- "帮我从《思考，快与慢》提取核心方法论"

### 2. 自动生成

Skill 会自动：
1. 搜索书籍的核心方法论
2. 整理方法论列表
3. 为每个方法论生成独立的 skill 文件
4. 提供安装和使用说明

### 3. 安装生成的 Skill

生成的每个方法论 skill 都可以独立安装和使用：

**OpenClaw:**
- 口语化安装：`帮我安装下 <skill-path>`
- 或使用命令：`npx skills add <skill-path>`
- 通过斜杠命令调用，如 `/mvp`

**Claude Code:**
- 复制到 `~/.claude/skills/` 目录
- 在对话中直接调用

**其他平台:**
- 根据平台要求安装到对应目录

## 示例:《精益创业》

已成功从《精益创业》(The Lean Startup) 中提取 10 个核心方法论:

1. **mvp.skill** - 最小可行产品
   - 触发: 准备开发产品，想用最低成本验证核心假设

2. **build-measure-learn.skill** - 构建-测量-学习循环
   - 触发: 想建立快速迭代的反馈循环

3. **validated-learning.skill** - 经证实的认知
   - 触发: 想通过数据而非直觉判断假设是否成立

4. **innovation-accounting.skill** - 创新核算
   - 触发: 想用可量化指标衡量创业进展

5. **pivot.skill** - 转型
   - 触发: 数据证明假设错误，需要调整方向

6. **five-whys.skill** - 五个为什么
   - 触发: 遇到问题，想找到根本原因

7. **hypotheses-validation.skill** - 价值假设与增长假设
   - 触发: 想验证产品和业务的可行性

8. **actionable-metrics.skill** - 避免虚荣指标
   - 触发: 想建立真正有意义的指标体系

9. **continuous-deployment.skill** - 持续部署
   - 触发: 想快速小批量推向用户

10. **lean-canvas.skill** - 精益画布
    - 触发: 想快速描述和验证商业模式

## 输出结构

```
examples/
└── 精益创业/
    ├── 方法论清单.md       # 所有方法论的总结文档
    ├── mvp/                # 最小可行产品 skill
    ├── build-measure-learn/ # 构建-测量-学习循环 skill
    └── pivot/              # 转型 skill
```

## 每个 Skill 的结构

每个生成的 skill 都包含:

- **name:** skill 的唯一标识符
- **description:** 触发场景和功能描述
- **适用场景:** 什么时候应该使用这个 skill
- **执行步骤:** 详细的操作步骤
- **输出格式:** 预期的输出内容和格式
- **注意事项:** 使用时需要注意的问题
- **来源:** 方法论的书籍来源

## 适用书籍类型

- 商业管理类书籍
- 个人成长类书籍
- 技术方法论类书籍
- 创业投资类书籍
- 其他包含系统方法论的书籍

## 注意事项

1. **书籍信息准确性:** skill 会通过网络搜索提取方法论,确保书籍名称准确
2. **方法论数量:** 如果书籍包含大量方法论,会优先提取最核心的 8-12 个
3. **安装选择:** 可以根据需要选择性安装部分 skill,不必全部安装
4. **持续优化:** 安装后可以根据实际使用情况,对 skill 进行优化调整

## 技术实现

- **搜索工具:** 使用 websearch 工具搜索书籍信息
- **信息提取:** 从多个来源提取和验证方法论
- **skill 生成:** 根据模板自动生成完整的 SKILL.md
- **打包工具:** 使用 skill-creator 的打包脚本生成 .skill 文件

## 作者

本 Skill 由 CymChad 开发，旨在帮助用户将书籍知识转化为可执行的 AI 工具。

## 贡献

欢迎贡献！请查看 [CONTRIBUTING.md](CONTRIBUTING.md) 了解如何参与。

## 版本历史

v1.0.0 - 2026-04-08
- 初始版本
- 支持从书籍提取方法论并生成 skill
- 成功测试《精益创业》案例
