---
name: lux-unity
description: "Unity automation commands for Lux CLI"
category: workflow
source: lux
source_path: Skills/lux-unity/SKILL.md
---

# LUX Unity

Use this skill only when a request directly involves operating or inspecting a Unity project through LUX.

## Core Rules

- Treat the project runtime directory as the runtime source of truth.
- Prefer explicit Unity automation commands over direct Unity project edits.
- Keep operations explicit, observable, and reversible where possible.
- Never hide automation, compile, test, or API failures behind fallback data.
- Read reference files only for the operation being performed.

## Operation References

- `references/backend-status.md` for automation backend status.
- `references/compile-tests.md` for compile and test flows.
- `references/dynamic-code.md` for guarded C# execution.
- `references/launch.md` for Unity launch behavior.
- `references/logs.md` for logs and event inspection.
- `references/object-hierarchy.md` for hierarchy/object inspection.
- `references/playmode-input.md` for play mode and input automation.
- `references/record-replay.md` for recording and replay.
- `references/screenshots.md` for screenshots and visual checks.

## Output

Report the command or API used, observed result, verification evidence, and any remaining blocker.
