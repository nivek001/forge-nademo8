# Forge Environment Report — Day 1

**Generated:** 2026-06-21T00:00:00Z  
**Hostname:** CBEN-1290YCX-LX  
**Engineer:** kevin.encarquez@accenture.com

---

## Tool Versions

| Tool | Version |
|------|---------|
| Claude Code | 2.1.185 |
| Node.js | v24.16.0 |
| Git | 2.54.0.windows.1 |
| ServiceNow SDK (`now-sdk`) | 4.7.2 |

---

## Skills Installed

- **Forge skills:** forge-author-skill, forge-blueprint, forge-bootstrap, forge-export, forge-fluent-catalog, forge-mcp-router, forge-package-kit, forge-scorecard, forge-sdk-catalog, forge-skill-updater, forge-standup, forge-start, remotemagic
- **GSD skills:** 67 `gsd-*` skills (v1.42.3)
- **Optional:** sn-workspace (installed)

---

## Remote MCP Configuration

| | |
|---|---|
| **Endpoint** | `servicenow-mcp.victoriouspebble-047683d1.westus2.azurecontainerapps.io` |
| **Instance** | `acnnademo8.service-now.com` |
| **Auth** | OAuth — stateless (login_id cached at `~/.claude/remotemagic/auth.json`) |
| **Status** | ✅ Connected |

---

## Smoke Test Transcript

**Test 1 — Incident count:**
```json
{ "status": "success", "table": "incident", "query": "(all)", "count": 19609 }
```

**Test 2 — Current scope:**
```json
{ "status": "success", "current_scope": { "sys_id": "global", "scope": "global", "name": "Global" } }
```

---

## Agent Operating Contract

- `.forge/AGENT-OPERATING-CONTRACT.md` — ✅ installed from Forge kit
- `.forge/SAFETY-CONTRACT.md` — ⚠️ missing (lead must commit from template)
- `CLAUDE.md` — ✅ wired with `@`-imports for both contracts

---

## Daily Auto-Update

- `Update-ForgeStack` function wired in PowerShell `$PROFILE` ✅
- Delegates to `/forge-skill-updater` (R4 compliant)
