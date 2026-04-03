# Ad Grant Clients

**Repo:** `growthpigs/ad-grant-clients`
**Created:** 2026-04-03

## What This Is

Per-client work for Google Ad Grant management. Each client gets a folder with their campaigns, content, analytics, and NPO documentation.

## Related Repos

| Repo | What It Is |
|------|-----------|
| `growthpigs/badaboost-ad-grants` | The service — methodology, SOPs, templates, knowledge |
| `growthpigs/google-ads-funnelizer` | The engine — code, APIs, scripts, content pipeline |
| This repo | Client work — deliverables, campaigns, content |

## Client Structure

Each client folder follows this pattern:

```
clients/[client-name]/
├── README.md           ← Client overview, contacts, account IDs
├── campaigns/          ← Ad campaigns, keywords, ad copy
├── content/            ← Blog posts, content clusters, infographics
├── analytics/          ← Reports, Clarity insights, performance data
├── npo/                ← NPO registration docs, Techsoup, G4NP
└── notes/              ← Meeting notes, handover, ongoing context
```

## Active Clients

| Client | Domain | Status | Monthly Fee |
|--------|--------|--------|-------------|
| **Retirementality** | retirementality.net | Active — needs funnel completion | Internal (own grant) |
| **ISKCON New Govardhan** | TBD (findkrishna.org exists) | Prospect — research phase | $500/mo target |

## Conventions

- Client folder names: kebab-case (e.g., `iskcon-new-govardhan`)
- One README.md per client with account IDs, contacts, current status
- Content clusters go in `content/clusters/`
- Campaign exports go in `campaigns/`
- No secrets in git — use `~/.claude/secrets/` for API keys

## Working with Clients

### Starting work on a client
1. Read their `README.md` for current state
2. Check `campaigns/` for active campaigns
3. Reference `growthpigs/badaboost-ad-grants` for SOPs
4. Use `growthpigs/google-ads-funnelizer` scripts for execution

### Adding a new client
1. Create `clients/[name]/README.md` with account details
2. Create subdirectories as needed
3. Add to the Active Clients table above
