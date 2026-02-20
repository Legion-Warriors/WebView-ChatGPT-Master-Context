# WebView ChatGPT Master Context

This repository is the working context and content state for an Android WebView engineering content series (LinkedIn/Twitter/Medium), plus generated post artifacts.

## Repository Structure

### Root Directory
- `README.md`
  - Repository guide and maintenance instructions (this file).
- `.gitkeep`
  - Placeholder file to keep the repository initialized when no other files exist in a new clone/template state.
- `CORE_CONTEXT.md`
  - Stable, long-lived context: objective, editorial rules, topic inventory, and strategic arc.
  - Update this only when foundational strategy/rules change.
- `CONTEXT_CHECKPOINT.md`
  - Full continuity checkpoint for recovering after context-window/session loss.
  - Includes legacy wrapper guidance and a full snapshot of progress/state.
- `SERIES_STATE.md`
  - Short mutable state for day-to-day continuity.
  - Tracks what is completed, what is next, and the operating template.
- `CHAT_TIMELINE_698bf088.md`
  - Condensed event timeline from the shared source chat.
  - Useful for provenance and decision traceability.
- `LinkedIn_Post_Hierarchy_Conversation.md`
  - Large source conversation and post hierarchy planning document.
  - Contains detailed decomposition (post order, hook-first release strategy, arc expansion).
- [`ANDROID_WEBVIEW_SERIES_ARCS.md`](ANDROID_WEBVIEW_SERIES_ARCS.md)
  - Arc-by-arc publishing roadmap across LinkedIn, Twitter/X, and Medium.
  - Tracks post sequencing, title direction, and current published/next state.
- `Hub-and-Spoke.md`
  - Technical reference note describing the hub-and-spoke hybrid architecture model.

### Content Directory
- `linkedin_posts/`
  - Stores finalized LinkedIn post files.
- `linkedin_posts/Post 1A`
  - Current saved LinkedIn artifact: "Inside Android WebView".

### Git Metadata Directory
- `.git/`
  - Version-control metadata managed by Git (branches, objects, refs, history).
  - Do not edit manually.

## How Files Work Together

1. Use `LinkedIn_Post_Hierarchy_Conversation.md` as the canonical source of truth.
2. Use [`ANDROID_WEBVIEW_SERIES_ARCS.md`](ANDROID_WEBVIEW_SERIES_ARCS.md) as the normalized execution subset of that source.
3. Use `CORE_CONTEXT.md` for stable strategy and constraints.
4. Use `SERIES_STATE.md` for quick “current status + next action.”
5. Use `CONTEXT_CHECKPOINT.md` when a full context restore is needed.
6. Save produced post outputs in `linkedin_posts/`.

## Maintenance Workflow

When adding a new post artifact:

1. Create/save the post file in `linkedin_posts/`.
2. Update `SERIES_STATE.md`:
   - Add completion line for the new artifact.
   - Update completed/next status.
3. Mirror the same checkpoint update in `CONTEXT_CHECKPOINT.md`.
4. If strategy or scope changed, update `CORE_CONTEXT.md`.
5. Commit all related files in one commit so state and artifact stay synchronized.

## Naming Conventions

- Post files: `linkedin_posts/Post <index><suffix>`
  - Example: `Post 1A`, `Post 2A`, `Post 2B`.
- Keep checkpoint wording explicit with date and file path for traceability.

## Current Snapshot (as of 2026-02-20)

- Completed artifact: `linkedin_posts/Post 1A`
- Checkpoint state updated in:
  - `SERIES_STATE.md`
  - `CONTEXT_CHECKPOINT.md`
