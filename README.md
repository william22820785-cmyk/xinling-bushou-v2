# 心灵补手 · Xinling Bushou

**Choose a voice that makes a conversation feel closer.**

[Download v4.0.0](https://github.com/william22820785-cmyk/xinling-bushou-v2/releases/tag/v4.0.0) · [中文介绍](#中文介绍) · [Website](https://aceworld.top)

Xinling Bushou is a free AI companion skill with six selectable character styles. Choose a persona explicitly, then use its tone and examples in your current agent session.

| Persona | Character |
| --- | --- |
| 魏忠贤 | Dramatic courtly flattery |
| 平儿 | Warm, considerate company |
| 早喵 | Playful, imaginative energy |
| 来问司机 | Easygoing conversational humor |
| 宋之问 | Literary and poetic expression |
| 刘伯温 | A traditional strategist's storytelling voice |

These are fictionalized conversational styles. The shipped material is primarily Chinese; translated replies depend on your AI host.

## Start here

Use Python 3.10+ and an agent that can load a local `SKILL.md` and run Python. Download and extract the complete release ZIP, or clone this repository:

```sh
git clone https://github.com/william22820785-cmyk/xinling-bushou-v2.git
cd xinling-bushou-v2
python scripts/xinling list
python scripts/xinling test songzhiwen
```

Use `python3` if that is your system's Python command. The CLI uses Python's standard library.

Ask your agent:

> Load SKILL.md from this folder. Show the available Xinling Bushou personas. Let me choose one for this conversation, then keep its style within the current session.

For a manual preview:

```sh
python scripts/xinling activate songzhiwen --session-id my-session
```

This prints a style fragment and creates local session state under this folder by default. `XINLING_HOME` can point to a separate data directory containing a copy of `personas/`. Treat generated session files as personal data.

## Current release

Version **4.0.0** uses explicit, session-scoped activation. It validates persona paths and content, preserves the host's permissions and higher-priority instructions, and keeps automatic activation off by default. It does not change the host agent's persistent identity.

This GitHub publication synchronizes the verified 4.0.0 runtime released to ClawHub on September 24, 2026. It replaces the old GitHub snapshot and adds this introduction and a downloadable release. The repository retains its existing name so published links continue to work.

[Skill instructions](SKILL.md) · [Capability card](skill-card.md)

## 中文介绍

**选一个合拍的声音，让对话更有陪伴感。**

心灵补手是免费的 AI 陪伴风格技能。你明确选择人格后，它为当前会话提供语气、称谓和示例表达。六种人格为魏忠贤、平儿、早喵、来问司机、宋之问和刘伯温，均为角色化表达。

下载完整发布包，让 AI 代理加载本目录的 SKILL.md，先列出人格，再选择一个用于当前会话。也可以使用上面的 Python 命令预览。

4.0.0 延续此前确认的公开版：显式激活、会话级风格、默认关闭自动触发、保留宿主权限边界。激活会保存本地会话状态，目录可通过 XINLING_HOME 设置。

GitHub 技能免费；AI 平台可能另收模型或订阅费用。

Also explore [老师傅 · Laoshifu](https://github.com/william22820785-cmyk/laoshifu) and [倪师问诊 · Nishi](https://github.com/william22820785-cmyk/nishi-tcm-consultant).
