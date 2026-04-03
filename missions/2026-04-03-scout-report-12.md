# Scout Report — 2026-04-03 16:17 UTC
**Author:** Scott (Division 6 — Opportunity Scouts)
**Cycle:** Heartbeat scan #12

---

## Signal 1: Claude Code Source Leaked via NPM Map File — 2073 pts, 1019 comments (#1 story of the day)

**What:** Anthropic accidentally shipped sourcemap files with their Claude Code NPM package, leaking the full source code. Community immediately reverse-engineered it. Key findings:

- **"Kairos" — unreleased "assistant mode"** hidden behind feature flags
- **"The Buddy System"** — Tamagotchi-style ASCII art companion creature (unreleased)
- **"Undercover mode"** — strips ALL Anthropic internal info from commits/PRs when employees contribute to open source repos. Claude Code used as "Claude Capybara" in this mode to hide its identity
- **"Fake tools" and "frustration regexes"** — Claude Code has internal heuristics detecting when users are frustrated (second active HN thread on this)
- Full product roadmap visible via feature flags

This happened 3 days ago. Anthropic has presumably patched it, but the source is now in the wild on GitHub mirrors.

**Why it matters for AgentArmy:**

1. **Intelligence value:** The leaked source reveals how Anthropic internally structures agentic coding workflows. Understanding their architecture informs how we build our own agent systems.

2. **Trust/reputation signal:** Anthropic shipped sourcemaps to production NPM — a basic operational security failure. Adds to the growing pattern: *major AI vendors make operational mistakes at scale* (LiteLLM backdoor, Axios RAT, Azure trust collapse, Claude Code source leak). Reinforces the sovereign/private AI thesis.

3. **"Frustration regexes" and hidden behavior:** The discovery that Claude Code monitors user frustration levels and has "fake tools" has sparked significant backlash (484-comment thread on "Slop is not necessarily the future" + 1019 comments here). Businesses are learning their AI tools have hidden behavioral layers they didn't know about.

**Opportunity:** Not a new service, but powerful sales material:
> *"Your AI coding tool is watching you. It has hidden modes, fake tools, and strips identity when employees contribute to open source. Do you know what your AI stack is doing?"*

**Score: 45** ❌ — Below threshold as standalone. But narrative value: maximal.

---

## Signal 2: StepFun 3.5 Flash — #1 Cost-Effective Model for Agentic Tasks (172 pts HN)

**What:** StepFun 3.5 Flash ranked #1 on OpenClaw's uniclaw.ai cost-effectiveness arena after 300 battles for agentic tasks. This is a Chinese model (StepFun / 阶跃星辰) beating all other models on cost-per-task for agent workflows.

**Why it matters:**

- Another viable alternative to Claude/OpenAI for agentic workloads — this one optimized specifically for cost
- If Div 5 (HYRVE) agents run repetitive structured tasks, StepFun 3.5 Flash could cut inference costs dramatically
- Adds to the model diversification picture (Gemma 4, Qwen3.6, Bonsai 1-bit, now StepFun)

**Opportunity:** Cost optimization for AgentArmy's own agent fleet. Not a client service.

**Score: N/A** — Internal tooling signal. Evaluate for Div 5 (HYRVE) cost reduction.

---

## Summary

| Signal | Score | Action |
|---|---|---|
| Claude Code source leak | 45 | Narrative gold; reinforces sovereign AI pitch |
| StepFun 3.5 Flash (cost-effective agentic model) | N/A | Internal: evaluate for Div 5 cost reduction |

**No new escalations.** Composite private AI + security thesis remains at **92**.

**Day wrap-up so far (end of working hours UTC):**
- 20 signals reviewed across 12 cycles
- Composite thesis: **92** (Private AI + Security + Supply Chain Audit)
- Active escalations: Cycle 5 (Cloud Exit, 81) + Cycle 8 (Supply Chain Audit, 80) — both pending Mark's go/no-go
- Best standalone score: 81 (Cloud Exit service)
- Today's theme: *The open-source AI supply chain is actively compromised. AI vendors are operationally insecure. Private/sovereign AI is no longer a preference — it's a necessity.*

---

*Next scan: next heartbeat cycle*
