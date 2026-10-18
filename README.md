# last-mile

> AI 做完了，不等于你拿到了。

一个 50 行的 Agent Skill：让 AI 在交付任何东西之前，先想一下你在哪、要干什么、以后还用不用，然后用最省事的方式递给你。

---

## 它解决什么问题

你跟 AI 说："帮我做个工具。"

它做完了，回你一句：

> 已完成，文件在 `E:\project\tools\copy-tool\main.py`，运行 `python main.py` 即可。

你得：打开文件夹 → 找到文件 → 打开命令行 → 敲命令 → 发现还得装依赖 → 回来问它。

**做完了，但你没用上。**

## 装上它之后

同样的任务，它会先想你这件事：

> **为什么这样给你**：这个工具你每天都要用，所以做成桌面图标，点一下就开。
> **你会看到**：桌面上多了一个「点评复制」图标。
> **你要做**：双击它。
> **不合适怎么换**：想放到别处、或者不要图标，说一声。

**能直接用的，才叫交付。**

---

## 它管什么，不管什么

只管一件事：**成品怎么到你手上。**

不管怎么做内容、怎么写代码、怎么剪视频。那些是别的技能和模型自己的事。

判断在任务过程中就做完了，不会等到最后拦你一下、问你要什么格式。

---

## 安装

```bash
git clone https://github.com/wy1040489623-tech/last-mile.git ~/.claude/skills/last-mile
```

各环境的技能目录：

```bash
# Claude Code
~/.claude/skills/last-mile/

# ZCode
~/.zcode/skills/last-mile/
```

装完新开一个会话生效。

## 使用

- **自动**：任务做完、准备交付时，自己触发。
- **手动**：`/last-mile`
- **点名**：直接说"按 last-mile 来"。

---

## 它很短，是故意的

五十行，没有脚本，没有依赖。

交付判断是一件"想起来就够"的事，不需要一套框架。写长了反而会被执行者忽略。

---

## 几个真实场景

见 [examples.md](examples.md)：做工具、做视频、发图到手机、一次性脚本，各自对比如今和装上之后的差别。

---

## License

MIT

---

# last-mile (English)

> Done is not delivered.

A 50-line agent skill: before handing anything to the user, the agent pauses and thinks about where they are, what they will do with it, and whether they will reuse it — then picks the lowest-friction way to hand it over.

## The problem

You ask an AI to build a small tool. It finishes and replies:

> Done. The file is at `E:\project\tools\copy-tool\main.py`. Run `python main.py`.

You then have to open the folder, find the file, open a terminal, run it, hit a missing dependency, and come back to ask again.

**It's finished, but you can't use it.**

## With last-mile

Same task. This time it thinks first:

> **Why this shape**: you'll use this every day, so it's a desktop icon — one double-click.
> **What you'll see**: a "Review Copy" icon on your desktop.
> **What you do**: double-click it.
> **If it doesn't fit**: say so and I'll move it or remove it.

**If the user can't use it immediately, it wasn't delivered.**

## What it does and doesn't do

It only handles **how the finished thing reaches the user**. It does not tell the model how to write, code, or edit — those belong to other skills.

The judgment happens while the work is being done, so the user is never interrupted at the end with a format question.

## Install

```bash
git clone https://github.com/wy1040489623-tech/last-mile.git ~/.claude/skills/last-mile
```

Skill directories by environment:

```bash
# Claude Code
~/.claude/skills/last-mile/

# ZCode
~/.zcode/skills/last-mile/
```

Start a new session to take effect.

## Use

- **Automatic**: triggers when work is done and about to be handed over.
- **Manual**: `/last-mile`
- **By name**: "use last-mile"

## It's short on purpose

Fifty lines. No scripts, no dependencies. Delivery judgment is a "remember to think" problem, not a framework. Long skills get ignored.

## Examples

See [examples.md](examples.md) for side-by-side comparisons across tools, videos, images, and one-off scripts.

## License

MIT
