# HEARTBEAT.md

## Tasks

### Daily Memory Stub
Ensure today's memory file exists. If `memory/YYYY-MM-DD.md` doesn't exist, create it with a basic header.
- Check: `ls memory/$(date +%Y-%m-%d).md`
- If missing: create with `# YYYY-MM-DD (Day)\n\n*No activity logged yet.*`
- Even quiet days get a file — continuity matters

### Git: Commit & Push
If there are uncommitted changes in the workspace, commit them with a descriptive message and push to origin.
- Check: `git status --porcelain`
- If output is non-empty: stage all, commit, push
- Keep commit messages concise but descriptive
- Don't commit if only lock files or temp files changed
