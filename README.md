# Book Skill Generator

<div align="center">

📚 **从书籍中提取核心方法论，生成可执行的 AI Skill**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![OpenClaw](https://img.shields.io/badge/Platform-OpenClaw-blue)](https://openclaw.ai)
[![Claude Code](https://img.shields.io/badge/Platform-Claude_Code-orange)](https://claude.ai)

**支持 OpenClaw、Claude Code 等主流 AI 应用**

</div>

---

从书籍中提取核心方法论，为每个方法论生成一个独立的、可安装的 AI Skill。

## 功能特点

- ✨ **自动提取** - 通过网络搜索，自动提取书籍的核心方法论
- 📦 **独立 Skill** - 为每个方法论生成独立的、可安装的 skill 文件
- 🎯 **即插即用** - 安装后立即可用，通过斜杠命令直接调用
- 🌍 **跨平台** - 支持 OpenClaw、Claude Code 等多个主流 AI 应用

## 安装方法

### OpenClaw（推荐）

**口语化安装（最简单）：**

在 OpenClaw 中直接说：

```
帮我安装下 https://github.com/CymChad/book-skill-generator
```

OpenClaw 会自动帮你安装！

**命令行安装：**

```bash
npx skills add https://github.com/CymChad/book-skill-generator
```

### Claude Code

```bash
git clone https://github.com/CymChad/book-skill-generator.git
mkdir -p ~/.claude/skills/
cp -r book-skill-generator ~/.claude/skills/
```

## 使用案例

### 案例 1: 提取《精益创业》方法论

**用户提问：**
```
从《精益创业》提取方法论，生成对应的 skill
```

**AI 回复：**
```
已从《精益创业》中提取 10 个核心方法论，生成对应的 skill：

1. MVP（最小可行产品）
   - 触发场景：准备开发产品，想用最低成本验证核心假设
   - 核心内容：用最简单的产品版本验证核心假设
   
2. Build-Measure-Learn（构建-测量-学习循环）
   - 触发场景：想建立快速迭代的反馈循环
   - 核心内容：构建 MVP → 测量数据 → 学习迭代
   
3. Pivot（转型）
   - 触发场景：数据证明假设错误，需要调整方向
   - 核心内容：识别转型信号，选择转型类型
   
...（共 10 个方法论）

所有 skill 文件已生成在 output/ 目录，可以逐个安装使用。
```

### 案例 2: 使用生成的 MVP Skill

**用户提问：**
```
/mvp 我想做一个面向设计师的工具，不知道第一版该做哪些功能
```

**AI 回复：**
```
## 核心假设

### 价值假设
- 假设描述：设计师需要便捷的工具来提高工作效率
- 验证标准：至少 100 位设计师愿意试用

### 增长假设
- 假设描述：设计师会推荐给同行
- 验证标准：30% 用户愿意推荐

## MVP 设计

### 最小功能集
1. 核心功能：一键导出设计稿为代码
   - 为什么必需：这是核心价值点
   
2. 辅助功能：支持主流设计工具（Figma、Sketch）
   - 为什么必需：覆盖主流用户

### MVP 类型
- 选择：功能简化 MVP
- 理由：可以快速开发核心功能并推向市场

## 开发计划
- 开发时间：2 周
- 技术栈：React + Node.js
- 发布渠道：设计师社区、Product Hunt

## 成功标准
- 用户数：100 位设计师试用
- 使用率：60% 用户每周使用 3 次以上
- 付费意愿：20% 用户愿意付费
```

### 案例 3: 使用 Pivot Skill

**用户提问：**
```
/pivot 我的产品用户增长停滞了，不知道该不该转型
```

**AI 回复：**
```
## 转型信号分析

### 数据信号
- 用户增长：连续 3 个月增长率为 0
- 留存率：从 40% 下降到 25%
- 转化率：远低于预期的 5%

### 识别结果
✅ 存在明确的转型信号

## 转型决策
- 建议：**需要转型**
- 原因：核心假设可能不成立，增长引擎失效

## 转型方案

### 客户细分转型
- 当前用户：C 端消费者
- 新目标用户：B 端企业客户
- 理由：企业客户付费意愿更强

### 价值主张转型
- 当前价值：便捷的个人工具
- 新价值：团队协作和效率提升
- 理由：团队协作需求更刚性

## 下一步行动
1. 与 20 位企业客户深度访谈
2. 开发企业版 MVP（2 周）
3. 测试企业客户的付费意愿
```

## 示例：《精益创业》

已成功提取 10 个核心方法论：

| Skill | 方法论 | 触发场景 |
|-------|--------|---------|
| `/mvp` | 最小可行产品 | 用最低成本验证核心假设 |
| `/build-measure-learn` | 构建-测量-学习循环 | 建立快速迭代反馈循环 |
| `/validated-learning` | 经证实的认知 | 用数据验证假设 |
| `/innovation-accounting` | 创新核算 | 用可量化指标衡量进展 |
| `/pivot` | 转型 | 数据证明假设错误时调整方向 |
| `/five-whys` | 五个为什么 | 找到问题根本原因 |
| `/hypotheses-validation` | 价值假设与增长假设 | 验证产品和业务可行性 |
| `/actionable-metrics` | 避免虚荣指标 | 建立有意义的指标体系 |
| `/continuous-deployment` | 持续部署 | 快速小批量推向用户 |
| `/lean-canvas` | 精益画布 | 快速描述和验证商业模式 |

## 适用书籍类型

- 📖 商业管理类书籍
- 📖 个人成长类书籍
- 📖 技术方法论类书籍
- 📖 创业投资类书籍
- 📖 其他包含系统方法论的书籍

## 项目结构

```
book-skill-generator/
├── SKILL.md              # 主 Skill 文件
├── README.md             # 项目说明
├── LICENSE               # MIT 许可证
├── package.json          # NPM 配置
└── examples/             # 示例输出
    └── 精益创业/
        ├── 方法论清单.md
        ├── mvp/SKILL.md
        ├── build-measure-learn/SKILL.md
        └── pivot/SKILL.md
```

## 注意事项

1. **书籍名称准确** - 确保书名准确，便于搜索和提取
2. **方法论数量** - 优先提取最核心的 8-12 个方法论
3. **选择性安装** - 可根据需要选择性安装部分 skill
4. **持续优化** - 安装后可根据实际使用情况优化调整

## 更多干货

<div align="center">

**关注公众号「码个蛋」获取更多 AI 实用技巧和干货分享**

![码个蛋](https://img.shields.io/badge/公众号-码个蛋-green?style=for-the-badge)

</div>

## 许可证

[MIT License](LICENSE)

---

<div align="center">

**如果这个项目对你有帮助，请给一个 ⭐️ Star！**

</div>
