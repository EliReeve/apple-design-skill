# Apple Design Skill

An agent skill that reviews your UI the way an Apple design reviewer would. It audits screens against the principles behind Apple's Human Interface Guidelines (clarity, deference, depth, consistency, accessibility) and returns findings with a reason and a concrete fix in whatever framework you're using: SwiftUI, UIKit, React, React Native, Flutter, Electron or plain HTML/CSS.

Built for Claude Code, Cursor, Codex and any agent that supports the Agent Skills format.

## What you get

- **Review mode.** Point it at a screen, a component or a screenshot and it returns a prioritised list: what's wrong, why it matters, and the fix.
- **Lenses.** Layout and spacing, typography, colour and contrast, touch targets, navigation, motion, dark mode, forms, onboarding, empty states, app icons, copywriting.
- **Cross-platform translation.** Apple terms mapped to the equivalent in each framework, so a finding about "navigation bar large titles" becomes an actual code change in React Native or Flutter.
- **Scored report.** Every review ends with a 1 to 5 score per lens so you can track a screen across iterations.

## Install

```bash
npx skills add EliReeve/apple-design-skill
```

Or clone into `~/.claude/skills/` (global) or `.claude/skills/` in a project.

## Use

```
Review this screen against Apple's design guidelines.
Audit the checkout form for accessibility and touch targets.
Check this page in dark mode and tell me what breaks.
Score the onboarding flow.
```

Narrow it with "Focus on typography" or "Only contrast issues".

## Structure

```
apple-design/
  SKILL.md              the review stance, lenses, report format
  references/
    lenses.md           what to check under each lens
    cross-platform.md   Apple term to framework equivalent
```

## Licence

MIT. Apple, the Human Interface Guidelines and all product names belong to Apple Inc. This project is independent and not affiliated with or endorsed by Apple.
