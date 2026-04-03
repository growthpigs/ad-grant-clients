# Retirementality

**Status:** Active — spending ~$8K/month, needs funnel completion + A/B testing
**Domain:** retirementality.net
**Type:** Internal (own grant)

## Account Details

| Field | Value |
|-------|-------|
| Google Ads Customer ID | 730-355-8944 |
| MCC | Badaboost Ad Grants (924-843-0199) |
| GA4 Property | 519180373 |
| GA4 Measurement ID | G-TBDJRLE4MX |
| GTM Container | GT-KFLDLD9V |
| Clarity Project | oydohki1wi |
| GHL Location | pcbUsSvoDMPrHHBcXpzq |
| Blog | blog.retirementality.net (BuildFast) |
| Quiz | quizapp-brown-two.vercel.app |
| Notion Blog DB | 1b307fa9108b808b8ef0f78255982a0c |

## Current State (as of 2026-04-03)

- **Spending:** ~$8K of $10K monthly grant
- **Conversions:** Only 6 — the problem is conversion, not spend
- **Blog:** 5 Coast FIRE articles live with infographics
- **Quiz funnel:** Deployed but needs A/B testing
- **Content pipeline:** `content-pipeline.py` working, GitHub Actions for Mon/Thu

## What Needs Doing

1. **Microsoft Clarity integration** — analyze user behavior, heatmaps
2. **A/B testing** — quiz funnel conversion optimization
3. **Funnel completion** — the full path from ad → blog → quiz → lead → GHL
4. **More content clusters** — expand beyond Coast FIRE
5. **CTR monitoring** — must stay >5% for compliance

## Funnel Architecture

```
Google Ad → Blog Article → Quiz CTA → quizapp (Vercel)
                                          ↓
                                    /api/lead endpoint
                                          ↓
                                  GHL API (creates contact)
                                  + GHL Webhook (triggers workflow)
                                          ↓
                                  Email to Hitesh + Contact tagged
```

## Team

- **Roderic** — Strategy, systems
- **Jono** — Account management (starting)
- **Sean** — WhatsApp group member

## Reference

Full engine config: `google-ads-funnelizer/accounts/retirementality/CONFIG.md`
