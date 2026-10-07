# AI Product Validator

A Claude Code skill: when a user describes a product requirement or idea, it first rationally evaluates "is this worth building" instead of jumping straight to building the product.

## Install

Clone into your personal skills directory:

```powershell
git clone https://github.com/yanyanwu458-png/ai-product-validator.git "$env:USERPROFILE\.claude\skills\ai-product-validator"
```

Linux / macOS:

```bash
git clone https://github.com/yanyanwu458-png/ai-product-validator.git ~/.claude/skills/ai-product-validator
```

## Usage

Describe your product idea and it will trigger the diagnosis, or run:

```
/ai-product-validator your product idea
```

## Output

Fixed format: `【Conclusion】` / `【Reasons】` / `【Verdict】` / `【Direction】`, keeping each answer under ~150 characters where possible.

## Structure & Extending

- 8 analysis dimensions, checked one by one.
- To add a dimension: append a numbered line to the "分析维度" list in `SKILL.md`; if it affects the verdict, also reflect it in the Reasons.
