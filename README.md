# Opsera Marketing Q1 FY2026 Dashboard

Live quarterly marketing report. Deployed via Opsera VIBEshift.

## Stack
- Static HTML dashboard
- Express.js (serves the file + `/health` endpoint for VIBEshift health checks)

## Deploy via VIBEshift
1. Push this repo to GitHub
2. In your IDE (Claude Code / Cursor / VS Code) with Opsera MCP wired up, send:
   > Use Opsera VIBEshift to deploy this repo to production.
3. The 6-step pipeline runs: stack detect → OAuth → Dockerfile → deploy → self-heal → health check
4. GitOps is on by default. Every push to `main` re-deploys.

## Local preview
```
npm install
npm start
# http://localhost:3000
```
