<div align="center">

# 🖕 fuck-you-and-stop-charging-for-sloppy-design-agents

### A Claude Code skill that actually designs beautiful UI.

**No subscriptions. No waitlists. No "AI-powered" landing pages that look like 2019 Bootstrap.**

Drop your design references → answer a few taste questions → get a complete design spec → then build unlimited production-quality UI from it. All inside Claude.

<br />

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-blueviolet)](#installation)
[![Stars](https://img.shields.io/github/stars/vb-tyagi/fuck-you-and-stop-charging-for-sloppy-design-agents?style=social)](https://github.com/vb-tyagi/fuck-you-and-stop-charging-for-sloppy-design-agents/stargazers)

</div>

---

## The Problem

Most "AI design tools or agents" today feel like paying a $20-50 monthly tax for mediocrity. They don't actually have "taste" - they just recycle the safest, most generic UI trends from 2021 and call it modern. Because these tools can't feel the difference between the surgical, sharp precision of Linear and the warm, approachable vibe of Notion, they just default to slapping gradients on everything. We're left with "soulless" interfaces that look like they were designed by a committee that hasn't seen a new idea in years. It's all pixels and zero personality.

## The Solution

One Claude Code skill that does two things:

1. **🔬 Decodes your design taste** — Reads designs you love (screenshots of *any* type — UI, graphic, 3D render, social creative, photo — or live URLs), one reference at a time, asks you smart questions, generates visual probes, and compiles a 12-section spec. Colors are **pinned from real pixels/CSS** (never eyeballed), every claim is **confidence-tiered**, and it captures the *why* behind each choice — not just the what.

2. **🏗️ Builds any UI from that spec** — Landing pages, SaaS dashboards, mobile apps, campaign pages, component libraries — all coded to YOUR aesthetic. Not some generic template. YOUR taste. And it runs an **anti-slop self-check** before delivering, actively refusing the generic defaults Claude drifts toward (Inter/Roboto, purple-gradient-on-white, card-grid monotony, fake-3D glass).

**Cost:** Whatever you already pay for Claude. That's it.

---

## What You Get

### Act I — Taste Extraction (~10-15 min)

```
Drop references → Answer 15 "would you rather" Qs → Review 4 design probes →
Refine with 4 more → Get a 12-section taste-spec.md
```

The spec includes:
- 🎨 **Pinned hex palette** — real values extracted from the pixels/CSS, not "dark theme" but `#0a0a0b`, `#141416`, `#1e1e21`, `#28282c` — each tagged with a confidence marker
- 🔤 **Named fonts** — not "expressive sans" but a concrete pairing with alternatives (and never a generic default unless your references genuinely use one)
- 📐 **Exact spacing** — not "generous" but `16px base, 24px related, 48px section, 96px major`
- 🚫 **Anti-goals** — bold "Never:" rules, including the named AI-slop defaults, that prevent the generic creep
- 🧭 **The WHY** — the taste rationale (trigger → decision → reason → trade-off) so the spec is transferable, not just descriptive
- 📋 **Two copy-pasteable AI prompts** — one for image-gen, one for product UI

### Act II — Unlimited UI Building

```
"Build the landing page" → production code
"Now the dashboard" → production code
"Mobile onboarding flow" → production code
"Settings page" → production code
"Dark mode variant" → production code
```

Every screen traces back to your taste spec. Consistency across 50 screens. One command per screen.

---

## Installation

### 1. Copy the skill file

```bash
mkdir -p ~/.claude/skills/fuck-you-and-stop-charging-for-sloppy-design-agents
curl -o ~/.claude/skills/fuck-you-and-stop-charging-for-sloppy-design-agents/SKILL.md \
  https://raw.githubusercontent.com/vb-tyagi/fuck-you-and-stop-charging-for-sloppy-design-agents/main/SKILL.md
```

### 2. That's it

Open Claude Code and say:

> "Extract my design taste"

Or:

> "I have a taste spec, build me a landing page"

Or just:

> `/fuck-you-and-stop-charging-for-sloppy-design-agents`

---

## How It Works

### Act I — The Taste Extraction Flow

| Phase | What Happens | Time |
|-------|-------------|------|
| **1. Onboard** | Tell it what you're building + your taste anchors (Apple? Linear? Notion?) | 1 min |
| **2. References** | Drop screenshots (any type) or paste URLs — it decodes each one at a time, pins real colors, reads live CSS where available | 2-3 min |
| **3. Questionnaire** | 10-15 "would you rather" questions. No jargon. A 16-year-old could answer them. | 3-5 min |
| **4. Probe Round 1** | 4 complete HTML/CSS pages generated — open them in your browser, rate them | 2-3 min |
| **5. Probe Round 2** | 4 refined variants based on your feedback — surgical differences | 2-3 min |
| **6. Compile** | Everything synthesized into `taste-spec.md` — 12 sections, all concrete values | Auto |

### Act II — The UI Building Loop

| Phase | What Happens |
|-------|-------------|
| **7. Lock spec** | Internalizes your taste spec (or accepts an existing one) |
| **8. Scope** | You say what to build — platform, tech stack, specific screen |
| **9. Constraints** | Applies platform rules (iOS safe areas, Web Vitals, a11y, touch targets) |
| **10. Build** | Generates production-quality code. Exact tokens from your spec. No approximations. |
| **11. Iterate** | "Change the hero spacing" → targeted edit. "Build the pricing page" → new screen, same spec. |

---

## The 25 Taste Axes

Your taste is measured across **5 categories, 25 dimensions**:

| Category | What It Measures |
|----------|-----------------|
| **Structure** | How space is organized — grid behavior, density, hierarchy, symmetry, rhythm |
| **Typography** | How text feels — drama, editorial vs functional, expression, scale, behavior |
| **Surface** | How things look — tactility, finish, borders, depth, warmth |
| **Color** | How color works — chromatic vs neutral, accent strategy, temperature, contrast |
| **Personality** | How it vibes — energy, system visibility, utility vs identity, tone, era, action |

---

## What The Probes Look Like

The skill generates **complete, self-contained HTML/CSS pages** — not wireframes, not mockups. Real pages you open in a browser.

Round 1 explores 4 wildly different directions:
- **Probe A**: Dark, spacious, editorial premium (think Linear)
- **Probe B**: Light, warm, organic (think Notion)
- **Probe C**: Dense, data-rich, power-user (think Bloomberg terminal meets modern UI)
- **Probe D**: Colorful, modern, energetic (think a well-designed startup)

Round 2 takes your favorite direction and makes 4 surgical variants — same family, different sub-styles.

---

## Platforms Supported

The UI builder applies **platform-specific constraints** automatically:

| Platform | What It Handles |
|----------|----------------|
| **Web / Landing** | Semantic HTML5, Core Web Vitals, responsive breakpoints, font loading |
| **Web App / SaaS** | Component isolation, WCAG AA, state handling, keyboard nav |
| **iOS** | Safe areas, 44pt touch targets, Dynamic Type, iOS nav conventions |
| **Android** | Material 3 (where compatible), 48dp targets, edge-to-edge, back gesture |
| **React Native** | Platform.OS checks, SafeArea, keyboard avoidance, FlatList optimization |
| **Flutter** | MediaQuery, SafeArea widget, theme extensions, const constructors |

---

## FAQ

**Q: Do I need API keys?**
A: You need Claude Code (which requires an Anthropic API key or Claude Pro/Max subscription). That's the only cost.

**Q: Can I skip taste extraction and just build UI?**
A: Yes. If you already have a design system doc or taste spec `.md` file, tell Claude "I have a taste spec, build me a landing page" and drop the file. It skips straight to Act II.

**Q: What tech stacks does it support?**
A: React + Tailwind (default), Next.js, Vue, plain HTML/CSS, React Native + NativeWind, Flutter, SwiftUI, Jetpack Compose — basically anything.

**Q: How is this different from v0, Bolt, Lovable, etc.?**
A: Those tools generate generic UI from a prompt. This tool first **understands your specific design taste** across 25 dimensions, then generates UI that's true to it. The difference is the same as between a random outfit and one picked by a stylist who studied your wardrobe.

**Q: Can I use the taste spec with other AI tools?**
A: Yes! Section 11 of the spec contains two copy-pasteable system prompts. Paste them into ChatGPT, Cursor, Copilot, v0 — anything. Your taste travels with you.

**Q: Why is it called "fuck you and stop charging for sloppy design agents"?**
A: Because someone had to say it. 🤷

---

## Contributing

The skill is one file: `SKILL.md`. PRs welcome for:

- Better questionnaire questions
- More platform constraints (Svelte, Astro, Solid, etc.)
- Additional taste axes
- Improved probe generation prompts
- Translations (the questionnaire is English-only right now)

---

## License

[MIT](LICENSE) — use it, fork it, improve it, ship beautiful things.

---

<div align="center">

**If you're tired of paying for AI design tools that don't understand taste, star this repo.**

<br />

*Built with rage and refined taste.*

</div>
