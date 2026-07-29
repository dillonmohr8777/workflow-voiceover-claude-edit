# Claude Code Instructions

Work only inside this repository unless Dillon Mohr explicitly expands the scope.

## Source-of-truth rules

- Never overwrite or modify `media/original/workflow-voiceover-original.mp4`.
- Treat the ChatCut project in `EDIT_MANIFEST.md` as the editable timeline source of truth for the current 9:18 cut.
- Put any new renders in `media/exports/` with a descriptive, versioned filename.
- Preserve `docs/workflow-voiceover-clean-transcript.md` as the readable transcript. If an edit changes timing or wording, create a new version rather than silently changing the current record.
- Update `EDIT_MANIFEST.md` whenever a new approved render is created.

## Editing requirements

- Preserve the substantive workflows, recommendations, examples, privacy warnings, and tool categories.
- Keep speech natural. Remove only filler, dead air, abandoned thoughts, repeated commentary, navigation chatter, interruptions, and explicit recording-control tails.
- Do not add music, sound effects, captions, branding, or synthetic voice unless Dillon asks.
- Preserve 1920×1080 framing unless a requested output targets another platform.
- Default delivery format: MP4, H.264 video, AAC audio, 30 fps.
- Check the start, midpoint, ending, sync, audio peaks, and full-frame scaling before declaring a render complete.

## Privacy and delivery

- This repository is private and contains internal workflow footage.
- Inspect for client, account, or organizational information before creating any shareable or public version.
- Do not publish, upload publicly, email externally, or change repository visibility without Dillon's explicit approval.
- Keep large media under Git LFS.

## Useful context

The video teaches account managers and other team members how to create personalized AI workflows using ChatGPT, Codex, role-specific integrations, Plan Mode, and supervised automation. The detailed content inventory is in `docs/workflow-voiceover-detailed-breakdown.md`.
