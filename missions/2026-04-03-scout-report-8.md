# Scout Report — 2026-04-03 15:17 UTC
**Author:** Scott (Division 6 — Opportunity Scouts)
**Cycle:** Heartbeat scan #8
**⚠️ ESCALATION — Score 90+ composite**

---

## Signal 1: Axios Compromised on NPM — 100M Weekly Downloads, RAT Dropper (1925 pts HN)

**What:** The most sophisticated open-source supply chain attack ever documented against a top-10 npm package. Axios (100M+ weekly downloads, the standard JavaScript HTTP client) had two malicious versions published to npm on March 30, 2026. The attack:

- Injected a fake dependency (`plain-crypto-js@4.2.1`) that deployed a full cross-platform Remote Access Trojan (RAT) across macOS, Windows, and Linux
- Connected to a live C2 server *within 2 seconds of `npm install`* — before npm finished resolving dependencies
- Self-destructed and replaced its own package.json with a clean decoy to defeat forensic detection
- Was staged 18 hours in advance. Three OS payloads pre-built. Both release branches poisoned within 39 minutes of each other
- **Zero malicious lines inside axios itself** — all in the injected dependency

Detected by StepSecurity's AI Package Analyst. Also hit the Backstage developer portal CI pipeline (12,000+ public repos using Harden-Runner).

**If you ran `npm install` between March 30–31 and got axios@1.14.1 or @0.30.4: assume compromised.**

**Why this matters for AgentArmy:**

1. **Immediate internal check needed:** Does any AgentArmy project use Node.js with npm? If so, verify axios version is not 1.14.1 or 0.30.4. Check all division codebases.

2. **Market opportunity — Supply Chain Security Service:** This is now the second major supply chain attack in one week (LiteLLM + axios). Both targeting the AI and developer ecosystems. This is a pattern, not a coincidence. Businesses are waking up to the fact that their entire Node.js/Python/npm/pip dependency chain is a live attack surface.

**Service offering:**
- "Supply Chain Security Audit" — scan client codebases for compromised or high-risk dependencies
- Automated: run `npm audit`, StepSecurity, Snyk, custom checks → report in 24h
- Ongoing: dependency monitoring subscription ($200–$500/mo for SMBs)
- Upsell: private AI deployment removes cloud AI dependency risk (connects to Cloud Exit thesis)

- **AI Leverage:** 10/10 — fully automatable, scripted scans + AI-generated report
- **Revenue Potential:** 8/10 — security spend is non-discretionary; every Node.js shop in the world is scared right now; fast sales cycle due to live threat
- **Score: 80** ✅ **ABOVE 75 — ESCALATE TO MARK**
- **Startup cost:** < $20/month (StepSecurity community tier is free, Snyk has free tier)

---

## ⚠️ Composite Security + Private AI Thesis: NOW 90

The full threat picture today:
| Attack Surface | Incident | Status |
|---|---|---|
| AI gateway | LiteLLM backdoored (Cycle 7) | Active threat |
| NPM ecosystem | Axios RAT dropper (this cycle) | Active threat |
| Cloud vendor | Azure trust collapse (Cycle 5) | Reputational |
| Platform surveillance | LinkedIn scanning extensions (Cycle 7) | Active |
| Model provider | OpenAI buying media co (Cycle 6) | Strategic |

**The unified pitch:** "You have four active attack surfaces in your tech stack right now. We audit and harden all of them."

Services:
1. Supply Chain Security Audit (npm/pip/AI dependencies) — $2K–$5K
2. Private AI Deployment (remove cloud AI risk) — $5K–$15K
3. Ongoing monitoring retainer — $500–$2K/month

This is one integrated product. Score: **90**.

---

## Summary

| Signal | Score | Action |
|---|---|---|
| Axios NPM RAT dropper | **80** | ⚠️ **Escalate to Mark** — standalone above threshold |
| Composite Security + Private AI | **90** | ⚠️ **Highest score of the day** |

**Internal action:** Verify AgentArmy codebases not running axios@1.14.1 or @0.30.4.

*Cumulative today: 14 signals, 8 cycles. Composite score: 90. Two active escalations pending Mark response.*

---

*Next scan: next heartbeat cycle*
