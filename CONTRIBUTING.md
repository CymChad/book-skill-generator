# 贡献指南

感谢你考虑为 Book Skill Generator 做贡献！

## 如何贡献

### 报告问题

如果你发现了 bug 或有功能建议：

1. 在 GitHub Issues 中搜索是否已有相关问题
2. 如果没有，创建新的 Issue：
   - 使用清晰的标题描述问题
   - 提供详细的复现步骤
   - 附上相关的日志或截图
   - 说明你的环境（操作系统、Node.js 版本等）

### 提交代码

1. **Fork 仓库**
   ```bash
   # 在 GitHub 上点击 Fork 按钮
   ```

2. **克隆你的 Fork**
   ```bash
   git clone https://github.com/你的用户名/book-skill-generator.git
   cd book-skill-generator
   ```

3. **创建分支**
   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **进行修改**
   - 遵循现有的代码风格
   - 添加必要的注释
   - 更新相关文档

5. **提交更改**
   ```bash
   git add .
   git commit -m "feat: 简短描述你的更改"
   ```

   提交信息格式：
   - `feat:` 新功能
   - `fix:` 修复 bug
   - `docs:` 文档更新
   - `style:` 代码格式调整
   - `refactor:` 代码重构
   - `test:` 测试相关
   - `chore:` 构建/工具相关

6. **推送到你的 Fork**
   ```bash
   git push origin feature/your-feature-name
   ```

7. **创建 Pull Request**
   - 在 GitHub 上打开你的 Fork
   - 点击 "New Pull Request"
   - 填写 PR 描述，说明你的更改内容和原因

### 分享书籍方法论

你可以分享你用这个 Skill 生成的书籍方法论：

1. 在 `examples/` 目录下创建书籍文件夹
2. 添加生成的 skill 文件和方法论清单
3. 提交 Pull Request

示例结构：
```
examples/
├── 小而美/
│   ├── 方法论清单.md
│   └── README.md
├── 精益创业/
│   ├── 方法论清单.md
│   └── README.md
└── 原子习惯/
    ├── 方法论清单.md
    └── README.md
```

## 开发指南

### 项目结构

```
book-skill-generator/
├── SKILL.md              # 主 Skill 文件
├── README.md             # 项目说明
├── LICENSE               # MIT 许可证
├── package.json          # NPM 配置
├── .gitignore           # Git 忽略文件
├── 发布指南.md           # 发布说明
├── CONTRIBUTING.md      # 本文件
└── examples/            # 示例输出
    └── 小而美/
        └── 方法论清单.md
```

### Skill 开发规范

#### SKILL.md 结构

```markdown
---
name: skill-name
description: 清晰描述何时触发和使用场景
---

# Skill 标题

## 核心理念
[一句话概括核心思想]

## 适用场景
- 场景 1
- 场景 2

## 执行步骤
### 步骤 1: [步骤名称]
[详细说明]

## 输出格式
[提供输出模板]

## 注意事项
- 注意点 1
- 注意点 2

## 来源
[方法论来源]
```

#### 命名规范

- **Skill 名称**: 使用小写字母和连字符，如 `find-community`
- **文件名**: 使用 `SKILL.md`（大写）
- **目录名**: 使用小写字母和连字符

#### 描述规范

- 清晰说明何时触发
- 包含具体的使用场景
- 避免过于技术化的术语
- 简洁但完整

### 测试

在提交 PR 之前，请测试你的更改：

1. **功能测试**
   - 使用不同的书籍名称测试
   - 验证生成的 skill 结构正确
   - 检查输出格式是否符合预期

2. **文档测试**
   - 检查文档链接是否有效
   - 验证示例代码是否可运行
   - 确保说明清晰易懂

## 代码规范

### Markdown

- 使用标准 Markdown 格式
- 标题层级清晰（最多 3 级）
- 代码块指定语言
- 列表项简短明确

### 注释

- 在复杂逻辑处添加注释
- 解释"为什么"而不是"是什么"
- 保持注释与代码同步更新

## 发布流程

维护者会定期发布新版本：

1. 更新 `package.json` 版本号
2. 更新 `CHANGELOG.md`
3. 创建 Git tag
4. 创建 GitHub Release
5. 推送到 GitHub

## 获取帮助

如果你有任何问题：

- 📖 查看 [README.md](README.md)
- 💬 在 [GitHub Discussions](https://github.com/你的用户名/book-skill-generator/discussions) 提问
- 🐛 在 [GitHub Issues](https://github.com/你的用户名/book-skill-generator/issues) 报告问题

## 许可证

通过贡献代码，你同意你的代码将以 MIT 许可证发布。

---

再次感谢你的贡献！🎉
