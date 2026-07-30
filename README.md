# Workflow Voiceover — Claude Editing Handoff

This public repository contains Dillon Mohr's workflow-training screen recording, the current full-length captioned master, the untouched source, the earlier short cut, a cleaned transcript, and a detailed topic-by-topic breakdown.

## Contents

- `media/original/workflow-voiceover-original.mp4` — untouched 15:43 source recording.
- `media/final/workflow-voiceover-full-uncut-momentum-3d-captions.mp4` — current 15:43 master with no cuts, Momentum blue-and-yellow 3D captions, and the official transparent M360 logo.
- `media/final/workflow-voiceover-edited-1080p.mp4` — earlier 9:18 cut, retained for reference.
- `docs/workflow-voiceover-clean-transcript.md` — cleaned readable transcript.
- `docs/workflow-voiceover-detailed-breakdown.md` — complete subject inventory and follow-up checklist.
- `EDIT_MANIFEST.md` — technical edit record and ChatCut project identifiers.
- `CLAUDE.md` — repository instructions for Claude Code.

Large video files are stored with Git LFS.

## Open the editable timeline

[Open the ChatCut project](https://app.chatcut.io/editor/65ddc230-1aec-4aaf-8aef-6bb604922a82?chatcutLaunchClient=codex_app&chatcutLaunchSurface=ext_browser)

The active timeline is `Full 15:43 — Momentum 3D Captions`.

## Clone for Claude Code

```powershell
gh repo clone dillonmohr8777/workflow-voiceover-claude-edit
Set-Location workflow-voiceover-claude-edit
git lfs pull
claude
```

## Current master

- Export duration: 15:43.000
- Source duration: 15:43.033
- Editorial cuts: none; the export omits only the final 0.033-second terminal frame to match the source audio boundary
- Exported source range: frame 0 through frame 28,289 at 30 fps
- Captions: 76px Montserrat, 900 weight, yellow fill, deep-blue outline, navy 3D extrusion, active-word highlight
- Logo: official transparent M360 orbit mark, 120×120px, full opacity, 28px from the lower-left edges
- Audio: original narration with timestamps normalized to start at 0.000 seconds; integrated loudness remains −12.9 LUFS
- Source format: 1920×1080, H.264 video, AAC audio
- Export format: 1080p MP4 (H.264), 30 fps

## Public-content warning

This repository is public at Dillon Mohr's explicit request. The recording includes internal workflow footage and may show organizational or client context. Review the footage before redistributing it or reusing excerpts.
