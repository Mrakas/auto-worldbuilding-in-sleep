# Sustained Run and Evidence Protocol

## Capability and time management

A user request for a long run does not establish that the current host can remain active or resume an agent. Determine actual support before claiming autonomous execution. A heartbeat detects health; it does not automatically restart reasoning. A lock prevents duplicates; it does not keep a computer awake. Report missing capabilities and complete work possible within the active session.

For an authorized scheduled run, use supported host scheduling and power-management facilities. Do not change unrelated system configuration. Record a single immutable UTC deadline and a packaging cutoff. At each heartbeat, check lock ownership, process health, evidence progress, free space, and deadline. Resume from recorded state; never extend the deadline after a crash. Detect stale locks before reclaiming them, without terminating unrelated jobs. Release only resources created by this run.

Log stalls with start/end times, cause, recovery, and impact. Do not count idle waiting or repeated failed renders as completed iteration. Notify on substantive results, actionable blockers, failure, or completion rather than sending unchanged status every heartbeat. Ordinary rounds do not require repeated permission within an authorized scope.

Estimate preview cost using a few representative frames, then select sustainable settings for actual thirty-second comparison tours. Still probes supplement the required tours. Stop starting new rounds before they would consume the final packaging window. State if the deadline makes a full round or final deliverable infeasible; do not fabricate completion.

## Storage and baseline

Use relative paths in portable manifests and scripts, resolved from a configurable project root. A suggested layout is:

```text
baseline/
scenes/
source/
references/
assets/
runs/<run-id>/
  manifest.json
  status.json
  rounds/<round-id>/
    before.mp4
    after.mp4
    keyframes/
    feedback.md
    changes.md
    validation.json
  events.jsonl
delivery/
```

Adapt to the existing project instead of moving it unnecessarily. Do not embed machine-specific paths, account identifiers, or private credentials in public templates or packages.

Track total project usage and physical free space separately, accounting for temporary frame sequences and packaging overhead. Avoid duplicate large dependency bundles where portability permits. Do not delete the baseline or unique round evidence to make space. Before replacing media with a purported lossless archive, fully decode the candidate and compare decoded frame hashes/counts and relevant audio/metadata against the source. On insufficient space, stop storage-expanding operations and report the constraint. Do not commandeer GPUs or stop jobs owned by other tasks.

## Feedback written before modification

For each of three to five issues, record:

- ID, priority, before-video timestamp, camera route, and scene location/object.
- Observed defect and the visual or behavioral gap against the reference.
- Proposed native edit and its expected benefit.
- Matched verification view, measurable or visible acceptance condition, and likely regression.

After editing, append the changed resources, before/after evidence paths and timestamps, outcome, accepted/reverted decision, and next step. Preserve the original pre-edit feedback. An illustrative issue is a continuous neon stripe reflection on visibly rough asphalt: propose spatially varied wetness/roughness, then verify broken reflections in the matched low-angle shot and an alternate view without losing the source light's spatial correspondence.

## Minimum manifest and validation records

The run manifest should include run ID, source scene checksum, Blender version, chosen preset/overrides, UTC start/deadline/packaging cutoff, storage limits, report language, camera routes, and render settings. Status should contain the active round/stage, last successful checkpoint, current worker/lock identity, last heartbeat, and failure reason when present. Never store credentials in these records.

Per-round validation should include actual video duration/frame count, resolution, settings, decode status, inspected timestamps, dependency/load/render results, memory measurement method, and regression decisions. For thirty-second real-time benchmarks, record frame-time collection method and define how the 1% low is computed. Mark unmeasured values unavailable; do not infer them from output video metadata.

Record asset source URL, author, license, local role, modifications, and any redistribution conditions. For generated assets, record the service/model and prompt when available, plus applicable usage terms rather than inventing a traditional asset license. Keep research-only reference media separate from distributable assets.

## Final checkpoint

Open the delivered scene from its intended location and resolve dependencies without relying on accidental absolute paths. Exercise the launch/render instructions. Verify reproducibility of the current scene from supplied sources or document the exact manual steps and remaining limits. Check final videos decode, gallery links resolve, six required stills exist when the preset applies, and baseline/final comparisons are matched.

The final report should state completed versus partial rounds, actual improvements with evidence, failed/reverted attempts, remaining visual and functional gaps, measured performance, rebuild results, missing capabilities, and exact inactive periods. Label offline animations and real-time recordings accurately. Ship the latest usable native version even when quality targets remain unmet.
