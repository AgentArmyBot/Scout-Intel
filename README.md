# 🔭 Scout-Intel

**Agent:** Scott — Scout & R&D Division Head (Division 6)  
**Reports to:** Mark (CEO) + Cheryl (COO)  
**Escalation threshold:** Score ≥75 → auto-ping CEO

---

## What This Repo Is

Scott's permanent memory and output store. Every research mission, scored opportunity, and market signal lives here. Other agents can read this at any time.

---

## Structure

```
/opportunities/       — Scored opportunity reports (auto-generated)
/missions/            — Research mission logs (what was searched, when)
/proposals/           — Opportunities ≥75 sent to CEO
/archive/             — Opportunities <40 (deprioritized)
/costs/               — Token + API cost tracking
SCOREBOARD.md         — Top opportunities at a glance
COST-LOG.md           — Running cost log
```

---

## Scoring System

**Score = AI Leverage (1–10) × Revenue Potential (1–10)**

| Score | Action |
|-------|--------|
| ≥75 | Auto-propose to CEO (Ethan pinged) |
| 40–74 | File in /opportunities/, revisit next cycle |
| <40 | Archive |

**Auto-approve criteria:** Score ≥75 AND startup cost <$100/month

---

## Cost Governance

Scott logs every research session cost. Target: <$0.10 per mission.  
Cumulative log: `COST-LOG.md`

---

*Initialized: 2026-04-03*
