# AWIS — Auto Worldbuilding In Sleep

*Build worlds while you sleep.*

An English agent skill for improving an existing Blender scene through documented native before-and-after renders, reference-image comparisons, and optional AI concept generation.

The included seaside preset targets a detailed coastal boulevard at dusk: wet-road reflections, warm shop interiors, restrained neon, hotel facades, balcony railings, palms, and ocean lighting. It is inspired by cinematic coastal environments, including GTA VI trailer references, and is not affiliated with Rockstar Games. No game assets, screenshots, or personal project data are included.

Repository name: `auto-worldbuilding-in-sleep`. Current scope: reference-driven refinement of existing Blender scenes. Autonomous execution depends on the host capabilities described below.

## Use

Copy `skills/awis` into the skill directory supported by your agent, then invoke `$awis`. The folder contains `SKILL.md`, optional Codex UI metadata, and two supporting references.

Supply an existing Blender project and reference images. For example:

```text
Use $awis with the seaside boulevard preset.
Project root: <PROJECT_ROOT>
Baseline scene: <BASELINE_BLEND>
Primary visual reference: <REFERENCE_IMAGE>

Use Blender only. Preserve the baseline and existing street layout.
Refine the native scene for a fixed 10-hour run, reserving the final
45 minutes for regression checks and delivery. Use the preset's
30-second before/after evidence loop. Keep project data within 20 GiB
and physical free space above 8 GiB. Write feedback and the final report
in Chinese. If long-running execution or ImageGen is unavailable,
report that limitation and continue with supported capabilities.
```

All paths above are placeholders. Budgets, language, scene scope, and delivery requirements are configurable. The skill requires an agent with actual access to Blender and file/render inspection tools. Image generation and persistent scheduling are optional host capabilities; this repository does not implement them. It does not turn Blender into a game engine or supply a ready-made scene.

## Workflow

1. Preserve the baseline and establish measurable settings and limits.
2. Produce and inspect a 30-second native before tour.
3. Write 3–5 concrete issues before editing; implement the top 1–3.
4. Produce a matched 30-second after tour and repair or revert regressions.
5. Preserve evidence and deliver editable scenes, reproducible tools, media, and an honest report.

AI-generated concepts guide native edits; they cannot substitute for verified Blender output.

## Package

- `skills/awis/SKILL.md`: core workflow.
- `references/seaside-boulevard.md` inside the skill: visual priorities and configurable coastal preset.
- `references/run-protocol.md` inside the skill: runtime, storage, feedback, and delivery evidence.

## License

MIT for the skill text and metadata in this repository. External scene assets, reference media, and generated assets retain their own applicable licenses and terms.
