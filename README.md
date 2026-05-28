# UX Builder Guidelines

AI 编码助手协作规则与 UX 交付规范模板。

## 文件结构

```
├── CLAUDE.md          # 全局行为原则（Karpathy 风格）
└── PROJECT_RULES.md   # UX 交付专项规则（按需读取）
```

## 使用方式

### Claude Code 全局配置

```bash
ln -s /path/to/ux-builder-guidelines/CLAUDE.md ~/.claude/CLAUDE.md
```

### opencode / Codex 全局配置

```bash
ln -s /path/to/ux-builder-guidelines/CLAUDE.md ~/.config/opencode/AGENTS.md
# 或
ln -s /path/to/ux-builder-guidelines/CLAUDE.md ~/.codex/AGENTS.md
```

### 项目级使用

直接在项目根目录放置 `CLAUDE.md`，末尾添加：

```markdown
---

全局行为原则见 `~/.claude/CLAUDE.md`。
UX 交付规范见 `~/.config/opencode/PROJECT_RULES.md`，遇到相关任务时主动读取。
```

## 背景

- **CLAUDE.md** — 借鉴 [Andrej Karpathy 的 CLAUDE.md](https://github.com/forrestchang/andrej-karpathy-skills) 风格，提炼 4 条行为原则：先思考、简洁至上、精确改动、目标驱动
- **PROJECT_RULES.md** — 来源于 UX 交付级代码原型规范，涵盖 TASK 拆解、Figma 还原、暗黑模式、质量测试、项目结构、交付清理
