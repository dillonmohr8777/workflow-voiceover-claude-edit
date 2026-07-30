# Claude Code Instructions

Work only inside this repository unless Dillon Mohr explicitly expands the scope.

## Source-of-truth rules

- Never overwrite or modify `media/original/workflow-voiceover-original.mp4`.
- Treat the `Full 15:43 — Momentum 3D Captions` ChatCut timeline in `EDIT_MANIFEST.md` as the editable source of truth for the current master.
- Treat `media/final/workflow-voiceover-full-uncut-momentum-3d-captions.mp4` as the current approved render.
- The 9:18 file is an earlier cut retained only for reference.
- Put new experimental renders in `media/exports/` with descriptive, versioned filenames.
- Preserve `docs/workflow-voiceover-clean-transcript.md` as the readable transcript. If an edit changes timing or wording, create a new version instead of silently changing the current record.
- Treat `docs/account-manager-ai-plugin-playbook.md` as the primary organization-wide report. Keep it role-neutral, preserve client separation and approval gates, and update its recording-coverage appendix if new transcript content is added.
- Update `EDIT_MANIFEST.md` whenever a new approved render is created.

## Editing requirements

- Preserve the entire 15:43 source unless Dillon explicitly requests a new cut. The current export boundary is frame 28,290 exclusive to avoid the source file's one-frame audio-duration mismatch.
- Preserve substantive workflows, recommendations, examples, privacy warnings, and tool categories.
- Do not remove words, pauses, or visual sections from the current master by default.
- Preserve the Momentum caption treatment unless Dillon requests a new style: bold Montserrat, yellow fill, deep-blue outline, navy 3D extrusion, active-word highlight.
- Preserve the official transparent M360 orbit logo at the lower-left corner unless Dillon requests a different placement.
- Do not add music, sound effects, branding, or synthetic voice unless Dillon asks.
- Preserve 1920×1080 framing unless a requested output targets another platform.
- Default delivery format: MP4, H.264 video, AAC audio, 30 fps.
- Check the start, midpoint, ending, sync, audio, caption readability, and full-frame scaling before declaring a render complete.

## Privacy and delivery

- The repository is public at Dillon Mohr's explicit request.
- The footage may include internal workflow, organizational, or client context.
- Do not send, publish, or distribute new versions beyond this already-approved public repository and Dillon's own Gmail without Dillon's explicit approval.
- Keep large media under Git LFS.

## Useful context

The video teaches Account Managers and other team members how to create repeatable AI workflows using ChatGPT, Codex, role-specific integrations, Plan Mode, and supervised automation. The generalized implementation report is `docs/account-manager-ai-plugin-playbook.md`; the source content inventory remains in `docs/workflow-voiceover-detailed-breakdown.md`.
