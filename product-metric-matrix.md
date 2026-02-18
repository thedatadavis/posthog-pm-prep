# PostHog AARRR Metrics Matrix: Complete Product Breakdown

## Matrix Structure Guide

**Key Definitions:**
- **Acquisition:** How users discover and sign up for each product
- **Activation:** The "aha moment" where users first experience value (within 14 days typically)
- **Retention:** Users continue using the product 3+ months after showing intent
- **Revenue:** Monetization metrics specific to product usage
- **Referral:** How users spread the product (internal team expansion + external)

***

## 1. PRODUCT ANALYTICS

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Signups showing Product Analytics intent<br>-  First pageview in product analytics dashboard<br>-  UTM source: organic search, competitor comparison pages | -  Time from signup to first analytics view<br>-  Source breakdown (SEO, paid, referral)<br>-  ICP vs. non-ICP acquisition ratio | -  60-70% of all signups show PA intent<br>-  <5 min from signup to first view |
| **Activation** | **Core Criteria:** Analyzed 2+ insights within 14 days<br>-  Created first trend/funnel/retention chart<br>-  Applied at least 1 filter<br>-  Viewed insights dashboard | -  Time-to-first-insight (TTFI)<br>-  Insights created per activated user<br>-  % using autocapture vs. custom events<br>-  Funnel creation rate | -  40-60% activation rate<br>-  80%+ retention for activated<br>-  <24 hours TTFI |
| **Retention** | -  Active users (viewed/created insight) 3 months after intent<br>-  Weekly Active Users (WAU)<br>-  Monthly Active Users (MAU)<br>-  Insights analyzed per week | -  WAU/MAU stickiness ratio<br>-  Cohort retention curves (Day 7, 30, 90)<br>-  Feature breadth (trends + funnels + retention)<br>-  % using HogQL for custom queries | -  70%+ 3-month retention<br>-  40-60% WAU/MAU ratio<br>-  Growing insights per user |
| **Revenue** | -  MRR from Product Analytics usage<br>-  Event volume-based pricing<br>-  Upgrade from free tier (1M events) | -  ARPU (Average Revenue Per User)<br>-  Events per $ (unit economics)<br>-  Free-to-paid conversion rate<br>-  Multi-product bundle attach rate | -  $500-$5k/mo per customer<br>-  8-15% free-to-paid conversion<br>-  50%+ use 2+ products |
| **Referral** | -  Teammate invitations from activated users<br>-  External mentions (blog posts, social)<br>-  Dashboard shares to external stakeholders | -  Team size growth (seats added)<br>-  Public dashboard shares<br>-  Community contributions (templates)<br>-  "Powered by PostHog" badge usage | -  2.5+ avg users per org<br>-  30% of orgs invite teammates |

***

## 2. SESSION REPLAY

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Clicked "Session Replay" in navigation<br>-  Viewed replay demo/documentation<br>-  Installed replay SDK/snippet | -  Source: error tracking need, UX research, PM request<br>-  Time from signup to replay intent<br>-  % discovering via Product Analytics | -  35-45% of signups show replay intent<br>-  Often 2nd product after analytics |
| **Activation** | **Core Criteria:** Watched 5+ recordings AND set a filter at least once<br>-  Applied filters (user properties, events, console errors)<br>-  Watched min 2 minutes total<br>-  Shared replay with teammate | -  Time-to-first-replay-watched<br>-  Filter types used (most common: errors, specific users)<br>-  % watching full sessions vs. skimming<br>-  Integration with product analytics (drill-down) | -  35-50% activation rate<br>-  75%+ retention for activated<br>-  <2 hours to first watched replay |
| **Retention** | -  Watched 5+ replays 3 months after intent<br>-  Weekly replay viewers<br>-  New recordings viewed per week | -  Avg replays watched per user per week<br>-  % linking replay to errors/flags<br>-  Rage click detection usage<br>-  Console log analysis engagement | -  75%+ 3-month retention<br>-  3-5 replays/user/week<br>-  Growing filter sophistication |
| **Revenue** | -  MRR from recording volume<br>-  Pricing tier based on recordings captured<br>-  Upgrade from free tier (5k recordings/mo) | -  Cost per recording<br>-  Recordings per customer<br>-  Multi-product bundle (replay + analytics + flags)<br>-  Feature flag integration revenue lift | -  $300-$3k/mo per customer<br>-  70%+ use with Product Analytics<br>-  40%+ use with Feature Flags |
| **Referral** | -  Engineers sharing replays with designers/PMs<br>-  Replay links shared in Slack/tickets<br>-  CS teams requesting replay access | -  Cross-functional user growth<br>-  Support ticket reply integration<br>-  External shares (customer support cases)<br>-  Replays embedded in bug reports | -  3-4 avg users per org<br>-  50%+ orgs add non-engineering users |

***

## 3. FEATURE FLAGS & A/B TESTING

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Clicked "Feature Flags" or "Experiments"<br>-  Viewed flags documentation<br>-  Installed flags SDK | -  Source: safe deployment need, experimentation need<br>-  % discovering via replay/analytics<br>-  Time from signup to flags intent | -  25-35% show flags intent<br>-  15-20% show experiment intent |
| **Activation** | **Feature Flags:** Deployed 3+ flags in production<br>**Experiments:** Launched 1+ experiment OR deployed 3+ flags<br>-  Analyzed experiment results in analytics<br>-  Used flag with rollout % (gradual deployment) | -  Time-to-first-flag-deployed<br>-  Flag types: boolean, multivariate, rollout<br>-  % using flags with analytics<br>-  Experiment statistical significance reached | -  30-40% activation (flags)<br>-  20-30% activation (experiments)<br>-  80%+ retention for activated |
| **Retention** | -  Active flags in production 3 months later<br>-  New flags created per month<br>-  Experiments run per quarter | -  % flags integrated with analytics<br>-  Kill switch usage (incident response)<br>-  A/B test velocity (tests/month)<br>-  Feature adoption via flags measured | -  80%+ 3-month retention<br>-  5-10 active flags per org<br>-  1-3 experiments/month |
| **Revenue** | -  MRR from flags usage<br>-  Pricing based on requests or seats<br>-  Experiment add-on revenue | -  Flags per customer<br>-  Experiment frequency<br>-  Multi-product attach (flags + analytics + replay)<br>-  Enterprise governance upsell (RBAC, audit logs) | -  $200-$2k/mo per customer<br>-  80%+ bundled with analytics<br>-  30% use experiments actively |
| **Referral** | -  PMs requesting flag access<br>-  Engineers sharing experiment results<br>-  Cross-team flag usage (backend + frontend) | -  User role diversity (eng, PM, design)<br>-  Flags shared across teams<br>-  Experiment insights presented in meetings<br>-  Internal advocacy for experimentation culture | -  2-3 avg users per org<br>-  40% invite non-engineering |

***

## 4. LLM ANALYTICS

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Clicked "LLM Analytics"<br>-  Viewed LLM docs/tutorials<br>-  Installed LLM SDK integration (OpenAI, Anthropic, etc.) | -  Source: AI feature launch, cost tracking need<br>-  % existing customers adding LLM tracking<br>-  Time from AI feature launch to tracking | -  8-12% of signups show LLM intent<br>-  Growing 15-20% MoM (2026) |
| **Activation** | **Core Criteria:** Tracked 100+ LLM events across 5+ users within 14 days<br>-  Viewed cost analysis dashboard<br>-  Created LLM-specific insight (token usage, latency)<br>-  Linked LLM event to user retention analysis | -  Time-to-first-LLM-event-tracked<br>-  Models tracked (GPT-4, Claude, custom)<br>-  % linking LLM to product analytics<br>-  Session replay + LLM integration usage | -  25-35% activation rate<br>-  70%+ retention for activated<br>-  <3 days to first 100 events |
| **Retention** | -  Actively tracking LLM events 3 months later<br>-  LLM events per week<br>-  Cost analysis viewed monthly | -  LLM usage trends over time<br>-  A/B testing prompts/models (via flags)<br>-  % correlating LLM usage to conversion/retention<br>-  Session replay analysis of AI UX | -  70%+ 3-month retention<br>-  10k+ LLM events/month<br>-  50%+ using with Product Analytics |
| **Revenue** | -  MRR from LLM event volume<br>-  Pricing per LLM event tracked<br>-  Free tier: 100k events/mo | -  LLM events per $<br>-  Multi-product bundle rate (LLM + analytics + replay)<br>-  Cost-per-customer LLM tracking<br>-  Enterprise AI compliance add-ons | -  $500-$5k/mo per customer<br>-  Higher than avg event volumes<br>-  90%+ bundled with analytics |
| **Referral** | -  AI/ML engineers inviting PMs<br>-  Product teams sharing AI impact analysis<br>-  External blog posts on AI observability | -  Cross-functional team growth<br>-  LLM insights shared in roadmap meetings<br>-  Community templates for LLM tracking<br>-  Conference talks mentioning PostHog LLM | -  2-4 avg users per org<br>-  High external advocacy (new category) |

***

## 5. SURVEYS & FEEDBACK

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Clicked "Surveys" in navigation<br>-  Viewed survey templates/docs<br>-  Created survey intent | -  Source: NPS tracking, qualitative research need<br>-  % PM-led orgs vs. engineer-led<br>-  Time from signup to survey interest | -  15-25% show survey intent<br>-  Often after analytics/replay |
| **Activation** | **Core Criteria:** Launched 1+ survey AND received 10+ responses<br>-  Analyzed survey results in analytics<br>-  Linked survey responses to user behavior<br>-  Created targeted survey (not broadcast) | -  Time-to-first-survey-launch<br>-  Response rate per survey<br>-  Survey types: NPS, CSAT, custom<br>-  % using behavioral targeting | -  30-40% activation rate<br>-  75%+ retention for activated<br>-  15-25% avg response rate |
| **Retention** | -  Active surveys running 3 months later<br>-  New surveys launched per quarter<br>-  Survey responses analyzed monthly | -  NPS/CSAT tracked over time<br>-  % correlating feedback to behavior<br>-  Session replay linkage (watch respondent)<br>-  Iterative survey improvements | -  75%+ 3-month retention<br>-  2-4 surveys per org/quarter<br>-  Growing behavioral targeting |
| **Revenue** | -  MRR from survey responses<br>-  Pricing per response collected<br>-  Free tier: 250 responses/mo | -  Responses per customer<br>-  Multi-product bundle (surveys + analytics + replay)<br>-  Qualtrics/Typeform replacement savings<br>-  Enterprise research program upsell | -  $100-$1k/mo per customer<br>-  80%+ bundled with analytics<br>-  Lower ARPU, high retention |
| **Referral** | -  PMs sharing survey insights with leadership<br>-  CS teams requesting survey access<br>-  Research teams adopting PostHog | -  User role expansion (PM → Researcher → Designer)<br>-  Survey templates shared in community<br>-  External case studies (survey → product change)<br>-  Integration with product decision docs | -  2-3 avg users per org<br>-  60% PM/product-led adoption |

***

## 6. ERROR TRACKING

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Enabled error tracking<br>-  Viewed errors dashboard<br>-  Installed error tracking SDK | -  Source: debugging need, production incidents<br>-  % discovering via session replay<br>-  Time from signup to error tracking | -  20-30% show error tracking intent<br>-  Often reactive (after incident) |
| **Activation** | **Core Criteria:** Tracked 10+ errors AND watched linked session replay for 1+ error<br>-  Set up error alerts<br>-  Grouped/resolved errors<br>-  Linked error to user profile | -  Time-to-first-error-captured<br>-  % linking errors to replays<br>-  Error volume per customer<br>-  Mean time to resolution (MTTR) improvement | -  35-45% activation rate<br>-  80%+ retention for activated<br>-  <1 hour to first error |
| **Retention** | -  Actively monitoring errors 3 months later<br>-  Errors captured per week<br>-  Errors resolved per month | -  Error trends (decreasing = product quality ↑)<br>-  % errors resolved with replay context<br>-  Alert responsiveness (time to acknowledge)<br>-  Integration with incident management | -  80%+ 3-month retention<br>-  Decreasing error rates over time<br>-  Fast MTTR (<2 hours) |
| **Revenue** | -  MRR from error event volume<br>-  Pricing per error tracked<br>-  Free tier: included in base product | -  Errors per customer<br>-  Sentry replacement savings<br>-  Multi-product bundle (errors + replay + flags)<br>-  Enterprise alerting/integrations | -  $200-$1.5k/mo per customer<br>-  90%+ bundled with replay<br>-  Competes with Sentry pricing |
| **Referral** | -  DevOps teams adopting for monitoring<br>-  Engineers sharing error dashboards<br>-  SRE teams requesting access | -  Cross-team adoption (eng → DevOps → SRE)<br>-  Integration with Slack/PagerDuty<br>-  External blog posts (debugging workflows)<br>-  Conference talks on replay-linked debugging | -  3-5 avg users per org<br>-  High engineer advocacy |

***

## 7. CUSTOMER ANALYTICS

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Viewed Customer Analytics dashboard<br>-  Accessed person/group profiles<br>-  Enabled B2B group analytics | -  Source: CS team need, account-level analysis<br>-  % B2B vs. B2C customers<br>-  Time from signup to customer analytics | -  30-40% show customer analytics intent<br>-  B2B orgs: 60-70% |
| **Activation** | **Core Criteria:** Viewed 10+ customer profiles AND created 1+ customer cohort<br>-  Integrated data warehouse (Stripe, HubSpot, Zendesk)<br>-  Used group analytics (for B2B)<br>-  Linked customer profile to replay/surveys | -  Time-to-first-profile-viewed<br>-  Data sources integrated (avg 2-3)<br>-  % using groups (B2B)<br>-  Customer health score created | -  35-45% activation rate<br>-  75%+ retention for activated<br>-  <2 days to first integration |
| **Retention** | -  Actively viewing customer profiles 3 months later<br>-  Profiles viewed per week<br>-  Customer cohorts analyzed monthly | -  Data warehouse usage growth<br>-  % CS teams using regularly<br>-  Customer health tracking sophistication<br>-  Expansion opportunity identification | -  75%+ 3-month retention<br>-  20-30 profiles viewed/user/week<br>-  3-5 active cohorts per org |
| **Revenue** | -  MRR from customer analytics usage<br>-  Data warehouse add-on revenue<br>-  Group analytics (B2B) pricing | -  ARPU for B2B vs. B2C<br>-  Data sources per customer<br>-  Segment + Amplitude replacement savings<br>-  CS team seat expansion | -  $1k-$10k/mo per customer<br>-  B2B higher ARPU (+50%)<br>-  60%+ multi-product bundle |
| **Referral** | -  CS teams sharing customer insights with sales<br>-  Account managers requesting access<br>-  Executive dashboards featuring customer data | -  Cross-functional adoption (product → CS → sales)<br>-  Executive presentation usage<br>-  Customer success case studies<br>-  Integration with CRM workflows | -  4-6 avg users per org<br>-  High cross-functional adoption |

***

## 8. DATA WAREHOUSE & CDP

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Enabled data warehouse<br>-  Connected first data source<br>-  Viewed CDP integrations (145+ sources) | -  Source: data consolidation need, analytics engineers<br>-  % existing customers adding warehouse<br>-  Time from signup to warehouse | -  15-25% show warehouse intent<br>-  Growing with enterprise customers |
| **Activation** | **Core Criteria:** Connected 2+ data sources AND ran 1+ HogQL query joining sources<br>-  Set up data pipeline/transformation<br>-  Created insights using warehouse data<br>-  Exported data to destination | -  Time-to-first-source-connected<br>-  Data sources connected (avg)<br>-  HogQL query complexity<br>-  ETL job success rate | -  25-35% activation rate<br>-  80%+ retention for activated<br>-  <1 week to first query |
| **Retention** | -  Actively querying warehouse 3 months later<br>-  HogQL queries per week<br>-  Data sources growing over time | -  Data warehouse usage sophistication<br>-  % building custom dashboards<br>-  ETL pipeline health<br>-  Query performance optimization | -  80%+ 3-month retention<br>-  5+ sources per org<br>-  10-20 queries/week |
| **Revenue** | -  MRR from data warehouse usage<br>-  Storage pricing<br>-  Query volume pricing<br>-  Rows synced per month | -  Storage per customer<br>-  Snowflake/BigQuery replacement savings<br>-  Reverse ETL add-on (Census/Hightouch replacement)<br>-  Enterprise data governance upsell | -  $2k-$20k/mo per customer<br>-  Highest ARPU product<br>-  90%+ enterprise customers |
| **Referral** | -  Analytics engineers advocating internally<br>-  Data teams migrating from Segment<br>-  Conference talks on warehouse-native analytics | -  Data team adoption<br>-  Migration from competitors (Segment, Firebolt)<br>-  Community SQL templates<br>-  Open-source contributions | -  3-5 avg users per org<br>-  High technical advocacy |

***

## 9. WEB ANALYTICS

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Enabled web analytics<br>-  Installed tracking snippet (cookieless)<br>-  Viewed web analytics dashboard | -  Source: GA4 alternative search, privacy concerns<br>-  % content/marketing sites vs. apps<br>-  Time from signup to web analytics | -  25-35% show web analytics intent<br>-  Often content/marketing teams |
| **Activation** | **Core Criteria:** Tracked 1,000+ pageviews AND analyzed 2+ web metrics (bounce rate, referrers, pages)<br>-  Set up UTM tracking<br>-  Created referrer analysis<br>-  Analyzed landing page performance | -  Time-to-1k-pageviews<br>-  % using cookieless tracking<br>-  UTM parameter coverage<br>-  Conversion tracking (web → signup) | -  40-50% activation rate<br>-  75%+ retention for activated<br>-  <7 days to activation |
| **Retention** | -  Actively tracking web analytics 3 months later<br>-  Pageviews per month<br>-  Web insights analyzed weekly | -  Traffic trends over time<br>-  % correlating web traffic to product signups<br>-  Funnel: web visitor → signup → activation<br>-  Content performance analysis | -  75%+ 3-month retention<br>-  50k+ pageviews/month<br>-  Growing traffic (content flywheel) |
| **Revenue** | -  MRR from pageview volume<br>-  Pricing per pageview/session<br>-  Free tier: 1M events/mo (generous vs. Plausible) | -  Pageviews per customer<br>-  GA4/Plausible replacement savings<br>-  Multi-product bundle (web + product analytics)<br>-  Marketing team seat expansion | -  $100-$500/mo per customer<br>-  Lower ARPU than product analytics<br>-  70%+ bundled with product analytics |
| **Referral** | -  Marketing teams sharing traffic analysis<br>-  Content teams using for editorial decisions<br>-  SEO teams adopting for rankings | -  Marketing team adoption<br>-  Content performance workflows<br>-  External case studies (GA4 migration)<br>-  Community templates (marketing dashboards) | -  2-3 avg users per org<br>-  Marketing-led referrals |

***

## 10. REVENUE ANALYTICS (BETA - 2026)

| AARRR Stage | Primary Metrics | Secondary Metrics | Target/Benchmark |
|-------------|----------------|-------------------|------------------|
| **Acquisition** | -  Enabled Revenue Analytics (beta)<br>-  Connected Stripe/payment data<br>-  Viewed revenue dashboard | -  Source: unit economics analysis, finance teams<br>-  % existing customers enabling beta<br>-  Time from signup to revenue analytics | -  5-10% show revenue analytics intent (beta)<br>-  Growing rapidly |
| **Activation** | **Core Criteria:** Connected payment data AND analyzed 1+ revenue metric (MRR, churn, LTV)<br>-  Correlated revenue to product usage<br>-  Calculated cost per acquisition (CPA) by source<br>-  Analyzed revenue by customer cohort | -  Time-to-first-revenue-insight<br>-  Payment systems integrated<br>-  % linking revenue to product events<br>-  Unit economics calculated | -  30-40% activation rate (early beta)<br>-  80%+ retention for activated<br>-  <3 days to integration |
| **Retention** | -  Actively analyzing revenue 3 months later<br>-  Revenue insights reviewed weekly<br>-  MRR/ARR tracking monthly | -  Revenue-to-usage correlation sophistication<br>-  % calculating LTV:CAC ratios<br>-  Churn analysis frequency<br>-  Expansion revenue tracking | -  80%+ 3-month retention<br>-  Weekly revenue review<br>-  Monthly board deck usage |
| **Revenue** | -  MRR from revenue analytics usage<br>-  Premium add-on pricing<br>-  Included in enterprise tier | -  ChartMogul/Baremetrics replacement<br>-  Multi-product bundle (revenue + analytics + customer)<br>-  Finance team seat expansion<br>-  Board reporting add-on | -  $500-$3k/mo per customer<br>-  High value-per-$ (C-level visibility)<br>-  90%+ bundled |
| **Referral** | -  Finance teams sharing revenue dashboards<br>-  CEOs presenting revenue analysis to boards<br>-  Investor updates featuring PostHog data | -  Executive adoption (CEO, CFO, VP Sales)<br>-  Board deck integration<br>-  External case studies (revenue impact)<br>-  VC portfolio company referrals | -  3-6 avg users per org<br>-  Highest executive visibility |

***

## CROSS-PRODUCT AARRR INSIGHTS

### Multi-Product Bundle Dynamics

**Activation Sequence (Most Common):**
1. **Product Analytics** (60-70% first product)
2. **Session Replay** (35-45% second product)
3. **Feature Flags** (25-35% third product)
4. **Customer Analytics / Surveys** (15-25% fourth product)
5. **LLM Analytics / Error Tracking / Data Warehouse** (specialty products)

**Key Retention Insight:** Customers using **3+ products have 2-3x higher retention** than single-product users.

***

### Universal AARRR Metrics (Company-Level)

| AARRR Stage | Company-Level Metrics | Target (2026) |
|-------------|----------------------|---------------|
| **Acquisition** | -  Total signups/month<br>-  ICP signups (high-growth startups)<br>-  Organic vs. paid vs. referral | -  15-20% MoM signup growth<br>-  40-50% ICP ratio<br>-  60%+ organic |
| **Activation** | -  Organizations activated for 1+ product<br>-  Multi-product activation (2+ products)<br>-  Teammate invitations (team activation) | -  50-60% org activation rate<br>-  30-40% multi-product activation<br>-  30% invite teammates |
| **Retention** | -  3-month retention (any product)<br>-  6-month retention<br>-  Cohort retention curves | -  70-80% 3-month retention<br>-  60-70% 6-month retention<br>-  Improving over time |
| **Revenue** | -  Monthly Recurring Revenue (MRR)<br>-  Annual Recurring Revenue (ARR)<br>-  Net Revenue Retention (NRR) | -  9-20% MoM MRR growth<br>-  120% half-yearly NRR target<br>-  $50M+ ARR (2026 target) |
| **Referral** | -  Word-of-mouth signups<br>-  Community contributions<br>-  Conference mentions<br>-  Public dashboards shared | -  30-40% signups from referral<br>-  Growing community<br>-  Top-of-mind for analytics |

***

## STRATEGIC AARRR PRIORITIES BY PRODUCT MATURITY

### Mature Products (Focus: Retention + Revenue)

**Product Analytics, Session Replay, Feature Flags**
- **Target:** 9-15% MoM revenue growth
- **Focus:** Retention optimization, feature depth, enterprise upsell
- **Key Metric:** Net Revenue Retention (NRR) 120%+

***

### Growth Products (Focus: Activation + Retention)

**Customer Analytics, Surveys, Error Tracking, Web Analytics**
- **Target:** 15-20% MoM revenue growth
- **Focus:** Activation improvement, product-market fit, cross-sell
- **Key Metric:** Activation rate + 3-month retention

***

### Emerging Products (Focus: Acquisition + Activation)

**LLM Analytics, Revenue Analytics (Beta)**
- **Target:** 20-30%+ MoM revenue growth
- **Focus:** Market education, product iteration, early adopter success
- **Key Metric:** Signups + activation rate + NPS

***

## PM ACTION ITEMS: AARRR OPTIMIZATION

### Monthly Checklist

**For Each Product You Own:**

1. **Acquisition Analysis**
   - [ ] Review signup trends (MoM growth)
   - [ ] Analyze acquisition sources (SEO, paid, referral)
   - [ ] Identify ICP vs. non-ICP ratio
   - [ ] Interview 1-2 new users about discovery journey

2. **Activation Deep Dive**
   - [ ] Check activation rate (target: 40-60%)
   - [ ] Review time-to-activation (decreasing = good)
   - [ ] Identify activation drop-off points (funnel analysis)
   - [ ] A/B test activation improvements

3. **Retention Monitoring**
   - [ ] Review 3-month retention (target: 70-80%)
   - [ ] Analyze cohort retention curves
   - [ ] Identify churn reasons (exit surveys, interviews)
   - [ ] Monitor usage trends (increasing engagement = good)

4. **Revenue Tracking**
   - [ ] Review MRR growth (mature: 9%+, growth: 15%+, emerging: 20%+)
   - [ ] Calculate ARPU and unit economics
   - [ ] Analyze free-to-paid conversion
   - [ ] Track multi-product attach rates

5. **Referral Cultivation**
   - [ ] Monitor teammate invitation rates
   - [ ] Track cross-functional user growth
   - [ ] Encourage community contributions
   - [ ] Highlight customer success stories

***

**Final Note:** PostHog's per-product activation framework means **every product gets its own AARRR funnel**. This granularity allows PMs to optimize each product independently while measuring cross-product synergies (e.g., Session Replay users who add Feature Flags have 2x retention).

The key insight: **Multi-product usage is PostHog's ultimate retention driver.** Every product should have a natural "integration point" that encourages users to discover and activate other products.
