---
name: unity-cs-reference
description: "Use https://github.com/islee23520/UnityCsReference as the Unity-specific reference basis for Unity Editor API decisions, not a generic C# language server. Prefer public UnityEditor APIs. Key areas: AssetDatabase import/GUID/path flow; BuildPipeline and BuildReport; CompilationPipeline and domain reload; EditorApplication events; UI Toolkit EditorWindow lifecycle; PackageManager requests; serialization and ScriptableObject persistence. Do not copy Unity implementation code."
category: workflow
source: lux
source_path: Skills/unity-cs-reference/SKILL.md
---

# Unity C# Reference

Use [UnityCsReference](https://github.com/islee23520/UnityCsReference) as the Unity-specific reference basis for Unity Editor API decisions. This skill is the Unity code-intelligence context for Lux; do not substitute generic C# language-server assumptions when the question depends on UnityEditor API shape, lifecycle, serialization, import, compilation, package, or build behavior.

Prefer public UnityEditor APIs. Key areas: AssetDatabase import/GUID/path flow; BuildPipeline and BuildReport; CompilationPipeline and domain reload; EditorApplication events; UI Toolkit EditorWindow lifecycle; PackageManager requests; serialization and ScriptableObject persistence. Do not copy Unity implementation code.

## Passive Loading Rule

Do not preload this skill during startup, hot reload, or background indexing. Read it only when the user request directly matches this workflow.

## Minimal Procedure

1. Confirm the target result and affected LUX subsystem.
2. Read only the files or evidence needed for the decision.
3. Apply the checklist above without expanding scope.
4. Produce concise output with evidence, risks, and the next verified action.

## Output

- Result or verdict.
- Evidence used.
- Risks or blockers.
- Verification performed or the smallest remaining check.
