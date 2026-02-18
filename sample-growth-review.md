## LLM Analytics — Monthly Growth Review (One-Page)

**Product:** LLM Analytics

**Stage:** Beta → GA → Early Growth

**Primary goal:** Make LLM Analytics a product engineers trust in production and can clearly tie to value (quality, cost, latency → product outcomes).

### 1) Executive story (what changed & why)

This month we saw **[activation / retention / revenue] move [up/down]**, driven primarily by **[integration friction / needle-finding value / pricing alignment]**. The strongest signal came from **[segment]**, while **[segment]** underperformed. Our current hypothesis is that **[X]**, not feature breadth, is the binding constraint.

---

### 2) Scoreboard (what we always review)

**Adoption & value**

* LLM intent rate (% orgs showing intent)
* Activation rate (≥100 LLM events + first insight within 14 days)
* Time-to-first-value (TTFV)
* 3-month retention (activated cohort)

**Behavioral depth (leading indicators)**

* % using filters / segmentation on traces
* % using evals or clustering
* % correlating LLM usage to product outcomes (conversion, retention)

**Commercial**

* LLM-attributed MRR or bundle uplift proxy
* Free → paid conversion among LLM-intent orgs
* Expansion vs contraction for LLM-using orgs

**Reliability & trust**

* Ingestion success rate / dropped events
* P95 query latency for core views
* Support tickets per activated org

---

### 3) Segments we always slice by

* Existing PostHog customer vs net-new
* SDK vs OpenTelemetry path
* AI-native product vs AI-adjacent feature
* Event volume tier (low / medium / high)
* Multi-product depth (1 vs 2+ vs 3+)

---

### 4) Key insights this month (example format)

* Activation is **X% lower** for Otel users → corroborated by interviews citing “unclear first step after data flows.”
* High-volume orgs retain but **don’t expand**, and often cap usage → pricing/value mismatch signal.
* Users who use **clustering or summaries** in week one have **~2× higher retention** than trace-only users.
* Support load spikes correlate with ingestion retries, not UI complexity.

---

### 5) Hypotheses we’re testing next (pick 2–4)

(See list below.)

---

### 6) Risks & watch items

* Activation drops masked by high early usage from AI-native teams
* Cost-to-serve increasing faster than perceived value for high-volume orgs
* “Looks powerful, feels overwhelming” UX risk as features GA

---

### 7) What success next month looks like (leading indicators)

* ↓ TTFV by X% for new activations
* ↑ % of orgs using ≥2 core capabilities
* ↓ support tickets per activated org
* Clearer willingness-to-pay signals (expansion or explicit limits)

---

## Potential Hypotheses (LLM Analytics)

### 1) Integration friction hypothesis

Activation is blocked not by missing features, but by **unclear “first useful question” after instrumentation**, especially for OpenTelemetry users.

Validation:

* Compare TTFV and activation between SDK vs Otel
* 3–4 interviews + trace ride-alongs
  Decision:
* Docs/wizard changes vs product changes

---

### 2) Needle-finding hypothesis

Users ingest data successfully but churn because they **can’t find meaningful signals in large trace volumes**.

Signal:

* Retention higher for users who use clustering/summaries early
  Decision:
* Invest in defaults + surfacing, not more ingestion features

---

### 3) Pricing-value mismatch (high-volume orgs)

High-volume orgs retain but cap usage or complain → pricing reflects **cost**, not **decision value**.

Signal:

* Usage plateaus without expansion
  Decision:
* Test value-based packaging (evals, summaries, alerts) vs raw event pricing

---

### 4) Feature breadth overwhelm

Early users activate but don’t deepen usage because **the mental model is unclear**.

Signal:

* High trace usage, low evals/clustering adoption
  Decision:
* Opinionated “starter path” rather than more knobs

---

### 5) AI-adjacent vs AI-native split

AI-adjacent teams need **correlation to product outcomes**, not observability depth.

Signal:

* Lower retention for AI-adjacent teams unless they link LLM data to product analytics
  Decision:
* Stronger cross-product workflows (LLM → conversion → retention)

---

### 6) Trust-breaker hypothesis

Small ingestion or latency issues disproportionately hurt retention because this is a **production-critical product**.

Signal:

* Support spikes precede churn
  Decision:
* Reliability work beats feature work this cycle

---

### 7) GA readiness mismatch

Some features are GA in name but not in **behavioral adoption**.

Signal:

* Features shipped, low repeated usage
  Decision:
* Delay GA framing; fix onboarding and defaults first

---

### 8) Multi-product leverage hypothesis

Retention jumps when LLM Analytics is used alongside Replay or Product Analytics, but discovery is accidental.

Signal:

* 2–3× retention for multi-product users
  Decision:
* Make integrations explicit and early in onboarding

---
