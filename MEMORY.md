# Memory Organization

## Structure

```
memory/
├── daily/           # 每日工作记录
│   └── YYYY-MM-DD.md
├── long-term/       # 长期知识库
│   ├── conventions.md      # 编码规范、约定
│   ├── decisions.md        # 重要决策记录
│   ├── lessons.md          # 经验教训
│   └── skills.md           # 技能清单
└── projects/        # 项目上下文
    └── <project-name>/
        ├── overview.md     # 项目概览
        ├── progress.md     # 进度跟踪
        └── notes.md        # 项目笔记
```

## Daily Records

每日记录格式：

```markdown
# YYYY-MM-DD

## Tasks
- [ ] 任务1
- [x] 任务2（已完成）

## Key Findings
- 发现1
- 发现2

## Notes
- 备注
```

## Long-Term Memory

### conventions.md
记录编码规范、工具使用习惯、项目约定等。

### decisions.md
记录重要决策，包括决策背景、选项分析和最终选择。

### lessons.md
记录经验教训，避免重复踩坑。

### skills.md
记录掌握的技能、工具组合、解决方案模式。

## Projects

每个项目一个目录，包含：
- **overview.md**：项目目标、技术栈、关键文件
- **progress.md**：里程碑、进度更新
- **notes.md**：开发过程中的思考和发现

## Access Pattern

1. 新对话开始时，先读取 `memory/long-term/conventions.md` 了解约定
2. 需要上下文时，读取相关项目的 `overview.md` 和 `progress.md`
3. 每天结束时，更新当日的 `daily/YYYY-MM-DD.md`
4. 重要发现归档到 `long-term/` 对应的文件