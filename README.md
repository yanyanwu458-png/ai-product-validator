# AI Product Validator

一个 Claude Code Skill：用户输入产品需求/想法后，先理性判断"这个需求值不值得做"，而不是直接帮用户做产品。

## 安装

克隆到个人 skills 目录：

```powershell
git clone https://github.com/yanyanwu458-png/ai-product-validator.git "$env:USERPROFILE\.claude\skills\ai-product-validator"
```

Linux / macOS：

```bash
git clone https://github.com/yanyanwu458-png/ai-product-validator.git ~/.claude/skills/ai-product-validator
```

## 使用

直接描述你的产品想法即可触发诊断，或输入：

```
/ai-product-validator 你的产品想法
```

## 输出

固定格式：`【结论】` / `【理由】` / `【判断】` / `【方向】`，每次回答尽量控制在 150 字以内。

## 结构与扩展

- 8 个分析维度，逐条核对。
- 扩展新维度：在 `SKILL.md` 的「分析维度」列表新增一行、编号递增即可；若新维度影响结论，需同步写进【理由】。
