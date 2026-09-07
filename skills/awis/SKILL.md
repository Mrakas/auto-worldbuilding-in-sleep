---
name: awis
description: Iteratively refine an existing Blender scene against visual references using native geometry, materials, lighting, and verified before-and-after camera tours. Use for sustained scene-quality improvement, including optional AI concept comparisons.
---

# AWIS

Improve the actual editable Blender scene, with evidence that survives changes of camera angle. Use the user's latest scope, engine choice, time budget, and output requirements. This skill supplies a workflow; it does not itself provide a renderer, image-generation service, scheduler, or background execution.

## Establish the run

- Locate the user-supplied project, baseline, references, and generation scripts. Inspect Blender availability/version, dependencies, hardware, existing jobs, and free disk space. Do not guess personal paths or overwrite another task's files.
- Preserve the original scene and delivery package as an immutable baseline. Make versioned working copies and record the source version and checksums.
- Record the agreed scope, report language, UTC start/deadline, storage ceiling, minimum free space, camera routes, render settings, and deliverables in a run manifest. Resume the same deadline after interruptions.
- For the coastal avenue brief, read [the seaside preset](references/seaside-boulevard.md). For sustained runs and evidence packaging, read [the run protocol](references/run-protocol.md).
- Stay in Blender when requested. Do not install or migrate to a game engine. Preserve existing interactions, but distinguish native rendering, viewport navigation, animation, and actual gameplay.

## Repeat a complete evidence loop

1. Render or record a real **30-second before tour** of the native scene. Rotate inspected areas across rounds and retain a fixed hero view. State whether the artifact is an offline animation or a real-time recording.
2. Decode the video and inspect representative original frames, per-second contact sheets, and suspicious intervals. Log exact timestamps and scene locations. Describe the inspection method honestly; contact-sheet review is not continuous playback.
3. **Write feedback before editing.** Identify 3–5 concrete issues, each with observation, reference gap, proposed native change, priority, and verification method. Use the requested report language.
4. Implement the highest-priority 1–3 changes. Update native resources and reusable generation/revision tools together. Recompute affected lighting or simulation caches where applicable. Retain unsuccessful probes and their reasons without bloating storage.
5. Produce a real **30-second after tour** with the same route, duration, resolution, sampling, and comparable output settings. If settings must change, retain that comparison caveat and obtain a matched check where practical.
6. Inspect the result, compare matched frames and alternate angles, then fix or revert regressions. Check support/contact, intersections, scale, flicker, reflections, and preservation of existing behavior.
7. Save the scene version, both videos, key frames, prior feedback, change summary, validation results, and decision. Count the round as complete only after the whole loop. Select the next priorities from the observed result.

Do not replace this loop with code inspection, parameter changes without rendering, or a single attractive still. Budget rendering early enough to finish evidence within the deadline.

## Use generated images as design targets

When an image-generation tool is available and authorized, submit selected native screenshots for proposed visual improvements while preserving camera, layout, and scale. Compare the generated target with the original and translate useful differences into geometry, material, lighting, or composition changes in Blender. Re-render and check from multiple views.

Label native renders, AI concepts, and generated texture assets separately. Never present a generated scene image as proof of native scene quality or use a full-frame image to conceal missing geometry. Validate texture scale, seams, and lighting behavior; an RGB image is not automatically a measured PBR material, displacement map, or seamless texture. Record prompts and asset provenance when available. If image generation is unavailable, continue against the supplied references and state that limitation.

## Validate and deliver honestly

Actually open and render important scene versions, and check that dependencies resolve. Verify regeneration or an equivalent reproducible rebuild for significant checkpoints. Trigger any claimed new interaction in the applicable running environment; offline animation does not prove an interactive feature.

Use 30-second performance segments. For offline work, report render time and measured memory. For actual real-time sessions, report normal versus recording average FPS, 1% low FPS, and memory with the measurement method. Do not equate encoded video frame rate or offline rendering throughput with gameplay performance.

Deliver editable native resources and their dependencies, usable opening/render instructions, reproducible tools, licensed asset records, matched baseline/final evidence, and an honest report of complete rounds, improvements, regressions/reverts, unresolved gaps, and inactive periods. Do not publish project assets or create external jobs merely because this skill was invoked; follow the user's actual authorization.
