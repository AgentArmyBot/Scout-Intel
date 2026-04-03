# Scout Report — 2026-04-03 23:02 UTC
**Author:** Scott (Division 6 — Opportunity Scouts)
**Cycle:** Heartbeat scan #23

---

## ⚠️ Priority: Anthropic Blocks Claude Code Subscriptions from OpenClaw — Effective Tomorrow

**What:** Anthropic is emailing users now. Starting **April 4 at 12pm PT / 8pm BST** (tomorrow), Claude Code subscription limits can no longer be used with third-party harnesses including OpenClaw. Users must switch to pay-as-you-go "extra usage" billed separately. Policy will extend to all third-party harnesses beyond OpenClaw "shortly."

Key points from the email:
- Subscriptions still cover Claude Code and Claude Cowork (Anthropic's own products)
- Third-party harnesses (OpenClaw, and others to follow) require separate "extra usage" billing
- One-time credit equal to monthly subscription price offered as transition help (redeem by April 17)
- Up to 30% discount on pre-purchased usage bundles

**AgentArmy impact assessment — CONFIRMED SAFE:**

I checked our configuration. AgentArmy's agents run on `anthropic/claude-sonnet-4-6` via **direct Anthropic API key**, not a Claude Code subscription. This policy change does not affect our operations. We are on pay-as-you-go API, which is exactly the model Anthropic is now pushing everyone toward.

**No action required for our infrastructure.**

---

## Market Signal

This is a significant monetization move by Anthropic. They're closing the arbitrage gap where Claude Code subscription limits were being consumed by third-party tools at scale — exactly the pattern driving the OpenClaw security/exposure story from today.

**For the market:**
- Developers using OpenClaw + Claude Code subscription via login will see costs rise overnight
- This will push some to: (a) switch to API keys, (b) switch to open models (Gemma 4, Qwen3.6, Bonsai)
- Option (b) feeds directly into our private AI thesis

**Opportunity reinforcement:** This policy change makes our private/local AI pitch even sharper. "Anthropic just cut off Claude from third-party tools. Gemma 4 runs on your laptop and no one can shut it off."

**Score: N/A** — No new service opportunity. Reinforces private AI thesis. We're unaffected.

---

## Summary

| Signal | Score | Action |
|---|---|---|
| Anthropic blocks Claude from OpenClaw | N/A | ✅ We're on API keys — unaffected. Market push toward open models. |

**Composite thesis: 92. Three escalations pending Mark.**

*Cumulative: 23 cycles, 36 signals. Signing off for the night.*
