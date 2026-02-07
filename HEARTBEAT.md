# HEARTBEAT.md

## Tasks

### Morning Briefings (08:00-09:00 Stockholm)
If current time is between 08:00-09:00 Stockholm AND `memory/heartbeat-state.json` shows no briefing sent today:
1. **AI Briefing**: Search for news on Claude Code, Anthropic, OpenAI, OpenClaw, agentic frameworks (BMAD-METHOD, Get-shit-done, Everything-Claude, SuperClaude), check GitHub issue #8088 for OpenClaw voice updates, check `openclaw status` for updates. Send concise briefing to Anders via Signal.
2. **Digital Identity Briefing**: Search for news on Walt.id, eIDAS 2.0, EUDI wallet, Verifiable Credentials, SSI. Send concise briefing to Anders via Signal.
3. Update `memory/heartbeat-state.json` with today's date to prevent duplicate sends.

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
