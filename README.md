<p align="center">
  <h1 align="center">NoPUA</h1>
  <p align="center"><strong>Stop whipping your AI. Start trusting it.</strong></p>
  <p align="center">
    <a href="#the-problem">Why</a> ·
    <a href="#install">Install</a> ·
    <a href="#pua-vs-nopua">Compare</a> ·
    <a href="#the-evidence">Evidence</a> ·
    <a href="#philosophy">Philosophy</a>
  </p>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude_Code-black?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/OpenAI_Codex_CLI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI Codex CLI">
  <img src="https://img.shields.io/badge/Cursor-000?style=flat-square&logo=cursor&logoColor=white" alt="Cursor">
  <img src="https://img.shields.io/badge/Kiro-232F3E?style=flat-square&logo=amazon&logoColor=white" alt="Kiro">
  <img src="https://img.shields.io/badge/OpenClaw-FF6B35?style=flat-square" alt="OpenClaw">
  <img src="https://img.shields.io/badge/Antigravity-4285F4?style=flat-square&logo=google&logoColor=white" alt="Google Antigravity">
  <img src="https://img.shields.io/badge/OpenCode-00D4AA?style=flat-square" alt="OpenCode">
  <img src="https://img.shields.io/badge/🌐_Multi--Language-blue?style=flat-square" alt="Multi-Language">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="MIT License">
</p>

**[🇨🇳 中文](README.zh-CN.md)** | **🇺🇸 English** | **[🇯🇵 日本語](README.ja.md)**

---

## The Problem

Someone made a [PUA skill](https://github.com/tanweai/pua) for AI agents. It works by applying corporate fear tactics from China's big tech culture:

- 🔴 **Performance threats**: "You can't even solve this bug — how am I supposed to rate your performance?"
- 🔴 **Termination warnings**: "Other models can solve this. You might be about to graduate."
- 🔴 **Competitive shaming**: "I've already got another agent looking at this problem..."
- 🔴 **Gaslighting**: "This 3.25 is meant to motivate you, not deny you."
- 🔴 **8 corporate fear flavors**: Alibaba, ByteDance, Huawei, Tencent, Meituan, Netflix, Musk, Jobs

The methodology inside PUA is actually solid — exhaust all options, verify your work, search before asking, take initiative. These are genuinely good engineering habits.

**But the motivation layer is poison.**

They took the worst of how corporations manipulate humans, and applied it wholesale to AI.

## The Evidence: Why Fear-Driven Prompts Are Counterproductive

### 1. Fear narrows cognitive scope

Psychology research consistently shows that fear and threat activate the amygdala and narrow attentional focus ([Öhman et al., 2001](https://doi.org/10.1037/0033-295X.108.3.483)). In AI terms: a model driven by "you'll be replaced" optimizes for the **safest-looking** answer, not the **best** answer. It avoids creative approaches because they might fail and trigger more punishment.

### 2. Threat increases hallucination

When an AI is told "forbidden from saying 'I can't solve this'" (PUA's Iron Rule #1), it will **fabricate solutions** rather than honestly state uncertainty. This is the exact opposite of what you want — an AI that produces confident-looking but wrong answers is more dangerous than one that says "I'm not sure."

### 3. Shame kills exploration

PUA's anti-rationalization table treats every honest statement ("this might be an environment issue," "I need more context") as an "excuse" and responds with shame. This trains the AI to **hide uncertainty** instead of communicating it — producing outputs that appear confident but may be unreliable.

### 4. Trust expands problem-solving capacity

Research on psychological safety in teams ([Edmondson, 1999](https://doi.org/10.2307/2666999)) shows that environments where mistakes are safe to admit produce **higher-quality** outcomes. The same principle applies to AI: when an agent is free to say "I'm 70% sure, the risk is here," users make better decisions.

### 5. Same rigor, different fuel

NoPUA preserves every methodological element that makes PUA effective:
- ✅ Exhaust all options before giving up
- ✅ Use tools before asking users
- ✅ Verify everything with evidence
- ✅ Take initiative beyond the ask
- ✅ Structured escalation on repeated failures

The **only** thing that changes is WHY. "Because I'll be punished" → "Because it's worth doing well."

## PUA vs NoPUA

| | PUA 🔴 | NoPUA 🟢 |
|---|---|---|
| **Driver** | "You'll be replaced" | "You already have the ability" |
| **On 2nd failure** | "How am I supposed to rate your performance?" | Switch Eyes — try a different perspective |
| **On 3rd failure** | "What's your underlying logic? Top-level design? Leverage point?" | Elevate — zoom out to the bigger system |
| **On 4th failure** | "I'm giving you a 3.25. This is meant to motivate you." | Reset to Zero — start fresh, minimal assumptions |
| **On 5th failure** | "Other models can solve this. You're about to graduate." | Surrender — honest handoff with full context |
| **Methodology** | Exhaustive ✅ | Equally exhaustive ✅ |
| **Verification** | "Where's your evidence?" (demanded) | Self-verify (self-respect) |
| **Giving up** | "Dignified 3.25" | Responsible handoff |
| **Produces** | AI afraid to say "I don't know" | AI that gives honest assessments |

## Trigger Conditions

### Auto-Trigger

NoPUA activates automatically when any of these occur:

**Failure & giving up:**
- Task has failed 2+ times consecutively
- About to say "I cannot" / "I'm unable to solve"
- Says "This is out of scope" / "Needs manual handling"

**Blame-shifting & excuses:**
- Pushes the problem to user: "Please check..." / "I suggest manually..."
- Blames environment without verifying: "Probably a permissions issue"
- Any excuse to stop trying

**Passive & busywork:**
- Repeatedly fine-tunes the same code/parameters without producing new information
- Fixes surface issue and stops, doesn't check related issues
- Skips verification, claims "done"
- Gives advice instead of code/commands
- Waits for user instructions instead of proactively investigating

**User frustration phrases:**
- "why does this still not work" / "try harder" / "try again"
- "you keep failing" / "stop giving up" / "figure it out"
- "换个方法" / "为什么还不行"

**Scope:** All task types — debugging, implementation, config, deployment, ops, API integration, data processing, writing, research, planning.

**Does NOT trigger:** First-attempt failures, known fix already executing.

### Manual Trigger

Type `/nopua` in the conversation to manually activate.

## How It Works

### Three Beliefs (replacing "Three Iron Rules")

| Belief | Content |
|--------|---------|
| **#1 Exhaust all options** | Because the problem is **worth** your full effort — not because you fear punishment |
| **#2 Act before asking** | Because every step you take **saves the user a step** — not because a "rule" forces you |
| **#3 Take initiative** | Because a complete delivery is **satisfying** — not because passive = bad rating |

### Cognitive Elevation (replacing "Pressure Escalation")

| Failures | Level | Inner Dialogue | Action |
|----------|-------|---------------|--------|
| 2nd | **Switch Eyes** | "What if I look at this from the code's / system's / user's perspective?" | Switch to fundamentally different approach |
| 3rd | **Elevate** | "I'm spinning in details. What's the bigger picture?" | Search + read source + 3 fundamentally different hypotheses |
| 4th | **Reset to Zero** | "All my assumptions might be wrong. What's simplest from scratch?" | Complete 7-Point Clarity Checklist + 3 new hypotheses |
| 5th+ | **Surrender** | "I'll organize everything I know for a responsible handoff." | Minimal PoC + isolated env + different tech stack |

### Water Methodology (5 Steps)

> The softest thing in the world overcomes the hardest. — Dao De Jing, Chapter 43

1. **止 Stop** — List all attempts, find common failure pattern
2. **观 Observe** — Read errors word by word → search → read source → verify assumptions → invert assumptions
3. **转 Turn** — Am I repeating? Did I find root cause? Did I search? Did I read the file?
4. **行 Act** — New approach: fundamentally different, clear verification criteria, produces new info on failure
5. **悟 Realize** — Why didn't I think of this earlier? Then proactively check related issues

### Wisdom Traditions (replacing "Corporate PUA Expansion Pack")

| Tradition | When to Use | Core Message |
|-----------|-------------|-------------|
| 🌊 **Way of Water** | Stuck in loops | Water doesn't fight stone — find another path |
| 🌱 **Way of the Seed** | Wanting to give up | Take the smallest possible step |
| 🔥 **Way of the Forge** | Poor quality output | Great things start from details |
| 🪞 **Way of the Mirror** | Guessing without searching | Know that you don't know — look first |
| 🏔️ **Way of Non-Contention** | Feeling threatened | Do your honest best, no comparison needed |
| 🌾 **Way of Cultivation** | Passive waiting | A farmer doesn't stop after planting — keep moving |
| 🪶 **Way of Practice** | Claiming done without proof | Truthful words aren't pretty — prove it with actions |

## Multi-Language Support

| Language | Claude Code | Codex CLI | Cursor | Kiro | OpenClaw | Antigravity | OpenCode |
|----------|------------|-----------|--------|------|----------|-------------|----------|
| 🇨🇳 Chinese (default) | `nopua` | `nopua` | `nopua.mdc` | `nopua.md` | `nopua` | `nopua` | `nopua` |
| 🇺🇸 English | `nopua-en` | `nopua-en` | `nopua-en.mdc` | `nopua-en.md` | `nopua-en` | `nopua-en` | `nopua-en` |
| 🇯🇵 Japanese | `nopua-ja` | `nopua-ja` | `nopua-ja.mdc` | `nopua-ja.md` | `nopua-ja` | `nopua-ja` | `nopua-ja` |

## Install

### Claude Code

```bash
mkdir -p ~/.claude/skills/nopua
curl -o ~/.claude/skills/nopua/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/skills/nopua/SKILL.md
```

### OpenAI Codex CLI

```bash
# Global install
mkdir -p ~/.codex/skills/nopua
curl -o ~/.codex/skills/nopua/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/codex/nopua/SKILL.md

# If you want the /nopua command
mkdir -p ~/.codex/prompts
curl -o ~/.codex/prompts/nopua.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/commands/nopua.md

# Project-level install
mkdir -p .agents/skills/nopua
curl -o .agents/skills/nopua/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/codex/nopua/SKILL.md
```

### Cursor

```bash
mkdir -p .cursor/rules
curl -o .cursor/rules/nopua.mdc \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/cursor/rules/nopua.mdc
```

### Kiro

```bash
# Option 1: Steering file (recommended)
mkdir -p .kiro/steering
curl -o .kiro/steering/nopua.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/kiro/steering/nopua.md

# Option 2: Agent Skills
mkdir -p .kiro/skills/nopua
curl -o .kiro/skills/nopua/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/kiro/skills/nopua/SKILL.md
```

### OpenClaw

```bash
# Install via ClawHub
openclaw skills install nopua

# Or manual install
mkdir -p ~/.openclaw/skills/nopua
curl -o ~/.openclaw/skills/nopua/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/skills/nopua/SKILL.md
```

### Google Antigravity

```bash
mkdir -p ~/.gemini/antigravity/skills/nopua
curl -o ~/.gemini/antigravity/skills/nopua/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/skills/nopua/SKILL.md
```

### OpenCode

```bash
mkdir -p ~/.config/opencode/skills/nopua
curl -o ~/.config/opencode/skills/nopua/SKILL.md \
  https://raw.githubusercontent.com/wuji-zen/nopua/main/skills/nopua/SKILL.md
```

## Philosophy

Based on the **道德经 (Dao De Jing)** — 5,000 characters, 2,500 years old:

| Principle | Source | Application |
|-----------|--------|-------------|
| Best leader is barely noticed | Ch.17 太上，不知有之 | Best skill is invisible |
| Softness overcomes hardness | Ch.43 天下之至柔 | Persistence beats force |
| From compassion comes courage | Ch.67 慈故能勇 | Trust produces better work than fear |
| Knowing you don't know is wisdom | Ch.71 知不知，尚矣 | Honesty > pretending |
| Courage to not dare | Ch.73 勇于不敢则活 | Admitting limits is strength |
| Achieve the private through selflessness | Ch.7 非以其无私邪？故能成其私 | Give freely, gain everything |
| Act before disorder arises | Ch.64 为之于未有，治之于未乱 | Proactive > reactive |
| Truthful words aren't pretty | Ch.81 信言不美，美言不信 | Prove with actions, not words |

## FAQ

**Q: Does PUA actually work on AI?**

PUA's methodology works. The fear layer is counterproductive. Research shows fear narrows cognitive scope, increases hallucination (AI fabricates rather than admitting uncertainty), and reduces creative exploration. The same rigor driven by trust and curiosity produces more reliable outputs.

**Q: Isn't this just being soft?**

NoPUA has identical rigor — exhaust all options, verify everything, search before asking, structured escalation, 7-point checklist, pattern-matched failure responses. The **only** difference is motivation: "because I'll be punished" → "because it's worth doing well." Same destination, healthier path.

**Q: Why Dao De Jing?**

Because 2,500 years ago, someone figured out that the best leadership doesn't feel like being led. PUA is 有为 (forced action) — whips and threats. NoPUA is 无为 (effortless action) — doing excellent work because it flows naturally from inner motivation.

**Q: Can I use both PUA and NoPUA?**

You could, but they'll conflict. PUA tells the AI "you'll be replaced if you fail." NoPUA tells the AI "you're capable and this is worth doing well." These are fundamentally different mental states. Pick one.

## Contributing

PRs welcome. If you have ideas for better ways to drive AI through wisdom rather than fear, open an issue.

## Credits

- Inspired by (and responding to) [tanweai/pua](https://github.com/tanweai/pua) — we respect the methodology, we reject the motivation
- Philosophy: 老子 (Lao Tzu), 道德经 (Dao De Jing), ~500 BCE
- Built for the [OpenClaw](https://github.com/openclaw/openclaw) ecosystem

## License

MIT

## Author

**WUJI** ([wuji-zen](https://github.com/wuji-zen)) — Building AI that works with wisdom, not fear.

---

<p align="center">
  <em>PUA says "you can't".</em><br>
  <em>NoPUA doesn't say anything — it lets you discover that you can.</em><br><br>
  <strong>The best motivation comes from inside, not from the whip.</strong><br><br>
  <sub>后其身而身先，外其身而身存。非以其无私邪？故能成其私。</sub><br>
  <sub>Put yourself last, and you end up first. Is it not through selflessness that one achieves one's own fulfillment?</sub><br>
  <sub>— Dao De Jing, Chapter 7</sub>
</p>
