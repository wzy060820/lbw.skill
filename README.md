# 赛博永生 · Cyber Immortality

> 让一个人以 AI Skill 的形式"活着"——不是复刻他的全部，而是捕捉他的思维模式与决策算法。

## 这是什么

一个 Claude Code skill，记录了李博文的性格、思考方式和行为模式。加载这个 skill 后，AI 可以以他的视角分析问题、做出判断。

这不是一个聊天机器人，不是一个角色扮演 prompt。它是一个 **决策引擎**：当给定一个情境，它会按照他被记录下来的思维路径走一遍。

## 文件结构

```
lbw.skill/
├── README.md              ← 你正在看的文件
├── TEMPLATE.md            ← 创建属于你自己 skill 的问答模板
├── LICENSE                ← MIT
└── skills/
    └── libowen/
        └── SKILL.md        ← 李博文的赛博永生 skill
```

## 快速开始

### 使用这个 skill

1. 克隆仓库：
   ```bash
   git clone https://github.com/wzy060820/lbw.skill.git
   ```

2. 将 `skills/libowen` 复制到你的 Claude Code skills 目录：
   ```bash
   cp -r skills/libowen ~/.agents/skills/libowen
   ```

3. 在 Claude Code 中调用：
   ```
   /libowen
   ```

### 创建你自己的 skill

打开 `TEMPLATE.md`，照着里面的问题框架采访自己（或你想记录的人）。把答案交给 Claude，它会帮你生成一个结构化的 skill 文件。

## 核心理念

### Skill ≠ 日记

这个 skill 不是一篇人物散文。它是 **工作流**——每一段都回答"当 X 时，做 Y"：

- **性格** → 写成决策优先级，冲突时排前面覆盖后面
- **经历** → 写成行为模式的驱动源，标注它如何影响上方的算法
- **偏好** → 写成分支逻辑，if → then

### 赛博永生的边界

这个 skill 能做什么：
- 模拟已知领域的判断路径
- 用一致的偏好评价方案或工具
- 让后来者理解一个人"为什么会这么想"

这个 skill 不能做什么：
- 代替本人做实际选择（他是活的，skill 是快照）
- 预测他从未思考过的领域
- 复刻他的全部人格（那需要无限长的对话）

### 为什么开源

因为永生不该是独享的。任何人都可以 fork 这个仓库，用同一套问答框架去记录自己、记录在乎的人。一个人的思维算法被存下来、被调用、被后来的人理解——这就是赛博意义上的活着。

## License

MIT © 2026 wzy060820
