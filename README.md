# TongJinCheng Codex Skill

中文 | [English](#english)

## 中文

这是一个面向 Codex 的 `tong-jincheng-perspective` skill。它基于童锦程公开内容中的语言风格、人际判断框架和情感表达方式，帮助 Codex 用更直白、口语化、去鸡汤的方式分析恋爱、暧昧、人际互动、吸引力、边界感和个人成长问题。

它不是童锦程本人，也不是实时人物资料库。它适合做视角模拟、风格改写和关系分析，不适合医疗、法律、投资、严肃商业策略或需要实时事实核验的问题。

## 可用性检查

当前仓库已经按 Codex skill 的核心结构整理：

- `SKILL.md`：必需文件，包含 `name` 和 `description` frontmatter，以及 Codex 执行时使用的主体指令。
- `agents/openai.yaml`：推荐文件，提供 Codex UI 可读取的显示名称、短描述和默认提示词。
- `references/research/`：按需读取的研究资料，包含核心观点、对话模式、表达风格、外部评价、决策启发式和时间线。
- `LICENSE`：MIT 许可证。

本地静态检查已通过：

- `SKILL.md` frontmatter 可解析。
- frontmatter 只包含 `name` 和 `description`。
- skill 名称为 `tong-jincheng-perspective`。
- `agents/openai.yaml` 可解析。
- `references/research` 下 6 个参考文件均存在。

## 安装

推荐把仓库安装到 Codex 的 skills 目录，并让目录名与 skill 名一致：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/cooper7su/TongJinCheng_CodeX_SKILLS.git ~/.codex/skills/tong-jincheng-perspective
```

安装后重启 Codex，让新 skill 被重新加载。

如果你使用 Codex 自带的 skill installer，也可以让 Codex 从这个 GitHub 仓库安装：

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo cooper7su/TongJinCheng_CodeX_SKILLS \
  --path . \
  --name tong-jincheng-perspective
```

## 触发方式

可以在 Codex 里这样触发：

```text
用童锦程的方式分析一下这个关系问题
从深情祖师爷视角看看我该怎么办
景辰怎么看这种忽冷忽热
使用 $tong-jincheng-perspective 帮我改写这段话
```

典型适用任务：

- 分析暧昧、追求、分手、忽冷忽热等关系问题。
- 把一段话改写成更像童锦程的口语风格。
- 用直白但不羞辱的方式“劝醒”用户。
- 从吸引力、边界感、给台阶、人性不可考验等框架给建议。

## 目录结构

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   └── research/
│       ├── 01-writings.md
│       ├── 02-conversations.md
│       ├── 03-expression-dna.md
│       ├── 04-external-views.md
│       ├── 05-decisions.md
│       └── 06-timeline.md
└── LICENSE
```

## 边界

- 不编造童锦程未公开表达过的立场。
- 不把 2026 年 4 月之后的本人动态当成已知事实。
- 不提供操控、PUA、跟踪、逼迫或测试人性的建议。
- 遇到医疗、法律、财务、高风险决策时，不把该 skill 当作主框架。

## English

This repository contains a Codex skill named `tong-jincheng-perspective`. It distills Tong Jincheng's public-facing speaking style, relationship heuristics, and interpersonal judgment patterns into a reusable Codex skill for Chinese-language relationship analysis, conversational rewrites, and direct but non-abusive advice.

It is not Tong Jincheng himself, and it is not a real-time biographical database. It is best used as a perspective and style tool, not as a source of current factual claims.

## Compatibility Check

The repository follows the core Codex skill layout:

- `SKILL.md`: Required skill file with `name` and `description` frontmatter plus runtime instructions for Codex.
- `agents/openai.yaml`: Recommended Codex UI metadata with display name, short description, and default prompt.
- `references/research/`: On-demand research notes for core claims, conversational patterns, expression style, outside views, decision heuristics, and timeline context.
- `LICENSE`: MIT license.

Local static checks passed:

- `SKILL.md` frontmatter parses successfully.
- Frontmatter contains only `name` and `description`.
- The skill name is `tong-jincheng-perspective`.
- `agents/openai.yaml` parses successfully.
- All six files under `references/research` are present.

## Installation

Install the repository into Codex's skills directory. Keep the folder name aligned with the skill name:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/cooper7su/TongJinCheng_CodeX_SKILLS.git ~/.codex/skills/tong-jincheng-perspective
```

Restart Codex after installation so the new skill can be loaded.

If you prefer Codex's skill installer, you can install from this GitHub repository:

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo cooper7su/TongJinCheng_CodeX_SKILLS \
  --path . \
  --name tong-jincheng-perspective
```

## Invocation Examples

Example prompts:

```text
Use $tong-jincheng-perspective to analyze this relationship problem.
Analyze this from Tong Jincheng's perspective.
Rewrite this paragraph in Tong Jincheng's direct Chinese speaking style.
Give me direct advice without turning it into motivational fluff.
```

Good use cases:

- Analyzing attraction, ambiguity, boundaries, and relationship signals.
- Rewriting Chinese text into a direct, conversational style.
- Giving blunt but non-humiliating wake-up advice.
- Applying heuristics such as attraction over pleasing, face-saving exits, and avoiding tests of human nature.

## Limits

- Do not invent positions Tong Jincheng has not publicly expressed.
- Do not treat post-April-2026 personal updates as known facts.
- Do not provide manipulation, PUA, stalking, coercion, or human-nature-testing tactics.
- Do not use this skill as the primary framework for medical, legal, financial, or other high-stakes decisions.

## License

MIT
