# HEARTBEAT.md

## Tasks

### Git: Commit & Push
If there are uncommitted changes in the workspace, commit them with a descriptive message and push to origin.
- Check: `git status --porcelain`
- If output is non-empty: stage all, commit, push
- Keep commit messages concise but descriptive
- Don't commit if only lock files or temp files changed
