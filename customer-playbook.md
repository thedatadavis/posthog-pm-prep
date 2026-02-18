# The PostHog Product Manager's Customer Playbook
## A Complete Mental Model for Understanding Who We Build For

***

## 1. FOUNDATIONAL PHILOSOPHY: Product-Minded Engineering Organization

### The PM's Role at PostHog (What Makes This Different)

**PostHog is NOT a traditional PM-led organization.** Engineers own sprint planning and solution spec'ing. PMs exist to **set context**, not to dictate roadmaps.

**Core PM Responsibilities:**
1. **Context Setting** - How products are being used, competitive landscape, user sentiment
2. **Growth Reviews** - Monthly reviews for products with PMF (Product-Market Fit)
3. **User Interviews** - Rule of thumb: **1 interview per week per PM**
4. **Product Coaching** - Teaching engineers "how to do product"
5. **Blind Spot Identification** - Research the "biggest unknowns" quarterly

**What PMs DON'T Do:**
- Set tasks for engineers (small teams are autonomous)
- Approve projects, expenses, or decisions
- Create career progression plans
- Manage HR or legal issues

**Mental Model:** Think of yourself as the **intelligence officer** for autonomous engineering units—you provide reconnaissance, competitive intel, and customer understanding so they can make better tactical decisions.

***

## 2. THE ICP FRAMEWORK: High-Growth Startups

### Primary ICP: High-Growth Startups

PostHog's **entire strategy flows from this definition.**

**Characteristics:**
- **Company Size:** 15-500 employees
- **Revenue:** $100k+/month OR very large consumer user base
- **Funding Status:** Raised from leading investors
- **Stage:** Post-PMF, pre-IPO
- **Growth Rate:** Quickly scaling customers, hiring, revenue

**Why This ICP Matters:**
1. **Efficient Monetization** - They have budget and can pay
2. **Quick Sales Cycle** - Self-serve motion, minimal friction
3. **Opinion Leaders** - Influence earlier-stage startups
4. **Strong Product Opinions** - Help us build better products
5. **Reference Customers** - Drive word-of-mouth growth

**Examples:**
- PostHog itself (Series B through IPO)
- Supabase
- ElevenLabs

### Secondary Segment: High-Potential Customers

**Definition:** Customers likely to **become** high-growth (e.g., PostHog during YC)

**Strategy:** Develop and nurture, but don't over-invest in customization

### Maintenance Mode: Hobbyists

**Definition:** Engineers building side projects

**Strategy:** 
- Provide excellent self-serve experience
- Don't actively market to them
- **Goal:** Be the first tool technical founders add to their product (so when they raise, they're already PostHog users)

***

## 3. PERSONA HIERARCHY: Evolution as Companies Scale

### The Persona Maturity Model

PostHog recognizes that **personas change as companies grow.** Each product should start with a single persona (usually early) and expand.

**Stage 1: Early Startup (0-15 employees)**
- **Primary Persona:** **Engineers** (Full-stack, Frontend, Backend)
- **Needs:** Fast setup, minimal instrumentation, developer-friendly UX
- **Product Usage:** Product Analytics, Session Replay, Feature Flags
- **Decision-Making:** Engineering makes buying decisions

**Stage 2: Scaling Startup (15-100 employees)**
- **Primary Persona:** **Product Managers**
- **Needs:** More sophisticated analytics, experimentation rigor, cohort analysis
- **Product Usage:** All core products + A/B testing, Revenue Analytics
- **Decision-Making:** PM + Engineering consensus

**Stage 3: Scale-Up (100-500 employees)**
- **Primary Persona:** **Analytics Engineers** / **Data Analysts**
- **Needs:** SQL access (HogQL), data warehouse integration, custom reporting
- **Product Usage:** Data Warehouse, CDP integrations, advanced querying
- **Decision-Making:** Data team + product leadership

### Persona Deep Dive by Product

Each small team may focus on different personas. **PM Heuristic:** Start narrow (one persona), expand only when that persona is well-served.

***

## 4. CUSTOMER NEEDS FRAMEWORK: The ICP Breakdown

### Things Our Customers **NEED** (Non-Negotiable)

**From PostHog's first ICP research:**

1. **Data Control & Privacy**
   - Need to self-host OR have clear data residency
   - GDPR/CCPA compliance
   - No data sharing with third parties
   - **Why:** Many in regulated industries or with privacy-conscious users

2. **Engineering-Led Decision Making**
   - Engineers choose tools, not procurement
   - Technical evaluation criteria matter
   - **Why:** PostHog is built for technical buyers who read docs and try the product

3. **Product-Market Fit Achievement**
   - They've found PMF and are scaling
   - **Why:** Pre-PMF companies churn; post-PMF companies need scalability and accuracy

4. **Self-Serve Capabilities**
   - Don't want to talk to sales to try the product
   - Want transparent pricing
   - **Why:** Developer culture values autonomy and transparency

5. **Scalability & Data Accuracy**
   - High event volumes (millions+)
   - Need reliable data for decision-making
   - **Why:** Post-PMF companies make critical decisions on data

### Things Our Customers **HAVE** (Common Attributes)

1. **Technical Sophistication**
   - Comfortable with code, APIs, SDKs
   - Higher bug tolerance IF we're fast and communicative
   - Appreciate SQL access (HogQL)

2. **Existing Tech Stack**
   - May have data warehouse (Snowflake, BigQuery)
   - Use modern dev tools (GitHub, Vercel, etc.)
   - Want integrations, not replacements

3. **Growth Orientation**
   - Focused on activation, retention, monetization metrics
   - Run experiments regularly
   - Data-informed decision culture

4. **Free Product Success** (Activation Signal)
   - Successfully used PostHog free tier
   - **PM Heuristic:** Free product success is the strongest PMF signal

### Things Our Customers **DON'T NEED** (Anti-Patterns)

1. **Enterprise Sales Process**
   - Don't need hand-holding or demos
   - Self-educate via docs
   - **Implication:** Feature-focused language, not benefit-focused

2. **Visual/No-Code Editors**
   - Don't need drag-and-drop builders
   - Comfortable with code-first workflows

3. **Marketing Attribution Tools**
   - Not optimizing ad spend (yet)
   - Product analytics > marketing analytics
   - **Implication:** Build SQL access before marketing dashboards

***

## 5. CUSTOMER JOURNEY MAPPING: From Free to Enterprise

### The PostHog Growth Funnel

**PM Mental Model:** PostHog is **product-led growth (PLG)** with sales assist for expansion.

#### Stage 1: Discovery & Signup
- **Trigger:** Technical founder/engineer searches for analytics tool
- **Touchpoint:** Website (unconventional, code-heavy, meme-filled)
- **Decision Factors:** 
  - Free tier (1M events/month)
  - Open-source credibility
  - Developer-friendly brand

#### Stage 2: Activation (Per-Product)
- **Critical PM Concept:** PostHog tracks **per-product activation** (not universal activation)
- **Why:** Users sign up with different needs (analytics vs. replay vs. flags)

**Per-Product Activation Criteria Structure:**
1. **Product Intent** - User shows interest (e.g., clicks "Session Replay")
2. **Activation Event** - User achieves "aha moment" (e.g., watches 5 replays with filters)
3. **Retention Check** - User returns 3 months later

**PM Heuristic for Setting Activation Metrics:**
- Not too easy (everyone activates but doesn't retain)
- Not too hard (no one activates)
- **Sweet spot:** ~40-60% activation rate with 80%+ retention for activated users

**Example Activation Criteria:**
- **Product Analytics:** Analyzed 2+ insights within 14 days
- **Session Replay:** Watched 5+ recordings AND set a filter
- **Feature Flags:** Launched 1+ experiment OR deployed 3+ flags
- **LLM Analytics:** Tracked 100+ LLM events across 5+ users

#### Stage 3: Expansion & Monetization
- **Free → Paid Trigger:** Hit usage limits OR need advanced features
- **PM Insight:** Free users who invite teammates have higher retention
- **Expansion Motion:** Add more products from the suite
- **CSM Engagement:** Assigned at ~$1.5M ARR per CSM

#### Stage 4: Retention & Advocacy
- **Success Metric:** 120% half-yearly Net Revenue Retention (NRR) target
- **PM Role:** Ensure activated users find continuous value
- **Churn Signals:** 
  - Declining engagement metrics
  - Not using multiple products (integration value missing)
  - Outgrowing PostHog's feature set (rare, but happens at enterprise scale)

***

## 6. METRICS FRAMEWORK: What PMs Track

### Growth Review Metrics (Monthly, Per-Product)

**Standard Metrics Across All Products:**

1. **Monthly Recurring Revenue (MRR)**
2. **Annual Recurring Revenue (ARR)**
3. **Month-over-Month Growth Rate**
   - Mature products: **>9% target**
   - Newer products: **15-20% average target**
4. **New Revenue Growth Rate**

**PM Heuristic:** These metrics are **standardized** so you can compare products and identify which need attention.

### Activation Metrics (Per-Product)

**Three-Part Structure:**

1. **Upfunnel:** Product intent shown
2. **Downfunnel:** Activation criteria met (within 14 days typically)
3. **Retention:** Product usage 3 months after intent

**PM Action:** If activation rate drops or retention declines, investigate with user interviews and session replays.

### Product-Market Fit Indicators

**Leading Indicators:**
1. **User Engagement Growth** - Growing faster than or in-line with signups
2. **Teammate Invitations** - Correlates strongly with retention
3. **Feature Adoption** - Using multiple PostHog products

**Lagging Indicators:**
1. **Retention Rates** - Especially cohort retention over 3-6 months
2. **Net Promoter Score (NPS)** - Tracking toward 40%+ "very disappointed" if lost
3. **ICP Customer Growth** - Number of paying ICP customers increasing

**PM Heuristic:** If engagement metric doesn't correlate to retention, either:
- You don't have PMF, OR
- You're tracking the wrong metric

### Revenue Quality Metrics

**Customer Lifetime Value (CLV) / Customer Acquisition Cost (CAC) Ratio:**

| Ratio | PMF Strength |
|-------|--------------|
| Over 3x | Very strong |
| 2x to 3x | Strong |
| 1.5x to 2x | Good |
| 1x to 1.5x | Promising |
| Under 1x | Weak |

**PM Insight:** PostHog's self-serve model means CAC should be low relative to CLV.

***

## 7. CUSTOMER SEGMENTATION: The Practical Breakdown

### Segment A: "The Ideal" - High-Growth B2B SaaS

**Profile:**
- 20-200 employees
- Post-Series A, pre-Series C
- Engineering-led culture
- $500k-$10M ARR
- Building for developers or technical users

**Products They Use:**
- Product Analytics (core)
- Session Replay (debugging)
- Feature Flags (shipping safely)
- A/B Testing (optimization)
- Error Tracking (reliability)

**PM Strategy:**
- **Optimize for this segment relentlessly**
- Build features they request
- Use them as reference customers
- Deep user interviews (weekly)

**Revenue Potential:** $10k-$100k ARR per customer

***

### Segment B: "The Aspirational" - AI/LLM Feature Teams

**Profile:**
- Traditional SaaS adding AI features
- 15-150 employees
- Recently integrated OpenAI/Anthropic
- Need to understand AI feature impact

**Products They Use:**
- LLM Analytics (new)
- Product Analytics (core usage)
- Session Replay (AI UX debugging)
- Feature Flags (A/B test models/prompts)

**PM Strategy:**
- **Emerging segment** - huge growth potential
- Position as "LLM analytics FOR PRODUCT TEAMS" (not AI-native companies)
- Emphasize business outcome connection (does AI drive retention?)
- Session Replay + LLM = killer combo

**Revenue Potential:** $15k-$80k ARR per customer (higher token volumes)

***

### Segment C: "The Data-Native" - Analytics Engineer Led

**Profile:**
- 100-500 employees
- Centralized data team
- Data warehouse in place (Snowflake/BigQuery)
- SQL-fluent users

**Products They Use:**
- Data Warehouse (integration)
- HogQL (SQL querying)
- CDP integrations (145+ sources/destinations)
- Product Analytics (custom reporting)

**PM Strategy:**
- Emphasize **HogQL flexibility** (custom queries)
- Highlight **warehouse-native** capabilities
- Compete against "best-of-breed" stacks (Segment + Amplitude)
- Focus on **total cost of ownership** savings

**Revenue Potential:** $50k-$300k ARR per customer

***

### Segment D: "The Scale-Up" - Mature Product Teams

**Profile:**
- 200-500 employees
- Product Managers + Analytics Engineers + Designers
- Multiple product lines
- Established processes

**Products They Use:**
- Full suite (Analytics, Replay, Flags, Surveys, Revenue Analytics)
- Group Analytics (B2B account-level)
- Customer Analytics Dashboard
- Data Warehouse + CDP

**PM Strategy:**
- **Account expansion** focus
- CSM-led relationship
- Build enterprise features (SSO, RBAC, audit logs)
- Risk: May outgrow PostHog and move to Amplitude + LaunchDarkly stack

**Revenue Potential:** $100k-$500k+ ARR per customer

***

### Segment X: "The Hobbyist" - Maintenance Mode

**Profile:**
- Solo developers
- Side projects
- No revenue or early revenue
- Free tier only

**Products They Use:**
- Product Analytics (basic)
- Maybe Web Analytics

**PM Strategy:**
- **Don't over-invest**, but provide excellent self-serve
- Goal: When they raise funding, they're already PostHog users
- Free tier is generous (1M events/month)

**Revenue Potential:** $0 currently, potential future value

***

## 8. PRODUCT-SPECIFIC CUSTOMER INSIGHTS

### Product Analytics Customers

**Persona Evolution:**
- **Early:** Engineers tracking basic metrics
- **Growth:** PMs building funnels and cohorts
- **Mature:** Analytics Engineers writing HogQL queries

**Key Customer Jobs:**
1. Understand user behavior
2. Measure feature impact
3. Build retention analyses
4. Calculate product metrics (DAU/MAU, activation, etc.)

**PM Insight:** Autocapture is the **moat** - customers don't want to manually instrument events.

***

### Session Replay Customers

**Primary Persona:** Engineers debugging issues

**Key Customer Jobs:**
1. Reproduce user-reported bugs
2. Understand UX friction points
3. Watch "rage clicks" and abandonment
4. Link errors to exact user sessions

**PM Insight:** **Replay-linked debugging** is unique - seeing console logs + DOM state + network requests in one view.

**Competitive Edge:** Integration with Feature Flags (see which experiment user was in) and Error Tracking (jump from error to replay).

***

### Feature Flags & A/B Testing Customers

**Primary Persona:** Product Engineers shipping features

**Key Customer Jobs:**
1. Ship features safely (gradual rollouts)
2. Run A/B experiments
3. Kill switches for incidents
4. Entitlement management

**PM Insight:** PostHog's advantage is **integration** - analyze experiment results in Product Analytics without exporting data.

**Competitive Weakness:** Less sophisticated than LaunchDarkly (enterprise governance, multi-env management).

***

### LLM Analytics Customers

**Primary Persona:** Product teams adding AI features (NOT AI-native startups)

**Key Customer Jobs:**
1. Track LLM API costs per user/cohort
2. Measure if AI features drive retention
3. Debug AI UX issues (slow responses, bad outputs)
4. A/B test prompts and models

**PM Insight:** **Unique positioning** - PostHog is the only LLM observability tool with native product analytics integration.

**Competitive Positioning:**
- **vs. Langfuse:** We connect LLM usage to business outcomes
- **vs. LangSmith:** We're for simple LLM features, not complex multi-agent systems
- **vs. Arize Phoenix:** We're managed + product-focused, not ML infra-focused

**Customer Segment Breakdown:**
- **Sweet Spot:** B2B SaaS adding chatbots, copilots, or generation features
- **Less Ideal:** AI-native companies building autonomous agents (they need Maxim AI, LangSmith)

***

### Surveys & Feedback Customers

**Primary Persona:** Product Managers seeking qualitative insights

**Key Customer Jobs:**
1. NPS/CSAT measurement
2. Feature request collection
3. User satisfaction tracking
4. In-app feedback loops

**PM Insight:** **Behavioral + attitudinal integration** is the moat - see survey responses linked to user's behavioral profile and session replay.

**Customer Use Case:** "User says they're confused → watch their session replay → see they never found the feature → add onboarding"

***

### Customer Analytics Customers

**Primary Persona:** CS teams and Product Managers

**Key Customer Jobs (B2C/B2B):**
1. Understand customer health
2. Identify expansion opportunities
3. Segment customers by behavior
4. Link customer profiles to revenue data (Stripe integration)

**B2B-Specific (Group Analytics):**
1. Account-level engagement tracking
2. User adoption within accounts
3. Feature usage by company
4. Account health scoring

**PM Insight:** **Unified customer view** - behavioral data + session replay + surveys + feature flags + LLM interactions in one profile.

**Competitive Edge:** CS teams can debug customer issues with full context (not just support tickets).

***

### Data Warehouse & CDP Customers

**Primary Persona:** Analytics Engineers and Data Teams

**Key Customer Jobs:**
1. Centralize data from multiple sources
2. Join PostHog data with CRM/payment data
3. Build custom dashboards
4. Export data for ML models

**PM Insight:** **Warehouse-native** approach - PostHog provides managed DuckDB warehouse that integrates natively with suite.

**Competitive Positioning:**
- **vs. Segment:** We're CDP + Analytics + Debugging (not just data routing)
- **vs. Snowflake:** We're managed and integrated (no ETL complexity)

***

## 9. CUSTOMER LIFECYCLE HEURISTICS

### Heuristic 1: Free Product Success = PMF Signal

**PM Rule:** If a customer successfully uses the free tier, they're likely ICP-fit.

**What "Success" Looks Like:**
- Reached activation criteria
- Invited teammates
- Used product for 3+ months
- Approaching usage limits

**PM Action:** Prioritize free tier experience - it's your PMF testing ground.

***

### Heuristic 2: Multi-Product Usage = Retention

**PM Rule:** Customers using 3+ PostHog products have significantly higher retention.

**Why:** Integration value kicks in - context switching elimination is the moat.

**PM Action:** 
- Encourage product discovery (in-app cross-promotion)
- Build workflows that span products (error → replay → flag status)
- Measure "product breadth" as a health metric

***

### Heuristic 3: Teammate Invitations = Retention Predictor

**PM Rule:** Users who invite teammates are more likely to retain.

**Why:** Indicates team adoption, not individual experiment.

**PM Action:** Optimize teammate invitation flow, track as activation sub-metric.

***

### Heuristic 4: High Engagement ≠ Revenue (Sometimes)

**PM Warning:** A customer can have high event volumes but low revenue potential if they're:
- Hobbyist with traffic but no business model
- Free tier maximizer with no intent to pay
- Using PostHog for non-core use case

**PM Action:** Segment by **ICP fit** first, then engagement. Track "ICP customer growth" separately from "total customer growth."

***

### Heuristic 5: "Very Disappointed" Cohort = PMF North Star

**PM Rule:** Track % of users who would be "very disappointed" if PostHog went away.

**Target:** 40%+ (Superhuman's benchmark)

**PM Action:** 
- Survey users quarterly
- Spend 50% of roadmap on improving for "very disappointed" cohort
- Spend 50% converting "somewhat disappointed" to "very disappointed"

***

## 10. COMPETITIVE CUSTOMER DYNAMICS

### Customer Decision Framework: PostHog vs. Alternatives

**PM Mental Model:** Customers evaluate PostHog against **stacks**, not single tools.

#### Decision Point 1: All-in-One vs. Best-of-Breed

**Customer Question:** "Do I want one platform or best-in-class for each category?"

**PostHog Wins When Customer:**
- Has small engineering team (<50 engineers)
- Values speed over perfection
- Budget-conscious ($20-50k vs. $200k+ for stack)
- Wants to minimize integrations/maintenance

**PostHog Loses When Customer:**
- Has dedicated data engineering team
- Needs enterprise governance (complex approvals, audit logs)
- Already invested heavily in existing stack (Segment + Amplitude)
- Requires deepest possible feature set in each category (e.g., LaunchDarkly's advanced flags)

***

#### Decision Point 2: Developer-First vs. Business-User-First

**Customer Question:** "Is this tool built for engineers or product/marketing teams?"

**PostHog Wins When Customer:**
- Engineering makes buying decisions
- Comfortable with code, SQL, APIs
- Values transparency (open source, pricing, data access)
- Prefers feature language over benefit language

**PostHog Loses When Customer:**
- Marketing-led organization
- Non-technical users need primary access
- Requires visual editors and no-code tools
- Deeply embedded in marketing stack (Google Ads, Salesforce)

***

#### Decision Point 3: Product-Led vs. Sales-Led

**Customer Question:** "Do I want to try before I buy, or need a sales process?"

**PostHog Wins When Customer:**
- Wants self-serve signup and trial
- Prefers transparent, usage-based pricing
- Evaluates via hands-on testing
- No procurement requirements

**PostHog Loses When Customer:**
- Enterprise procurement process required
- Needs extensive demos and POCs
- Wants custom pricing negotiations
- Multi-department sign-off required

***

### Customer Churn Analysis Framework

**PM Playbook:** Categorize churn into **preventable** vs. **natural evolution**

#### Preventable Churn

**Reason 1: Failed Activation**
- User signed up but never reached "aha moment"
- **PM Action:** Improve onboarding, lower activation friction

**Reason 2: Missing Key Feature**
- Customer needed specific functionality PostHog lacks
- **PM Action:** Evaluate if feature fits ICP needs (don't chase feature requests from non-ICP)

**Reason 3: Data Quality Issues**
- Events not capturing correctly, data inaccuracies
- **PM Action:** Prioritize reliability and accuracy (table stakes for post-PMF companies)

**Reason 4: Poor Support Experience**
- Bugs not fixed quickly, questions unanswered
- **PM Action:** PostHog values "fast and communicative" over "bug-free" (ICP has high bug tolerance IF we respond quickly)

#### Natural Evolution Churn

**Reason 1: Outgrew PostHog**
- Customer scaled to enterprise (500+ employees) and needs enterprise features PostHog doesn't prioritize
- **PM Acceptance:** Not every customer stays forever; focus on ICP retention

**Reason 2: Pivoted Away from ICP**
- Customer shifted to enterprise sales motion, now needs marketing attribution tools
- **PM Acceptance:** They left ICP; focus on keeping ICP customers

**Reason 3: Acquisition/Shutdown**
- Company acquired or shut down
- **PM Acceptance:** External factor

***

## 11. CUSTOMER RESEARCH PRINCIPLES

### The "1 Interview Per Week Per PM" Rule

**Why This Matters:**
- PMs set context - you MUST talk to customers regularly
- Interviews reveal jobs-to-be-done that data can't show
- Builds empathy and product intuition

**PM Heuristic:** If you're not doing 1 interview/week, you're not doing your job.

***

### Who to Interview

**Prioritization Framework:**

1. **"Very Disappointed" Cohort (40%+)** - Your power users, understand what they love
2. **"Somewhat Disappointed" Cohort** - Understand blockers to becoming "very disappointed"
3. **Churned ICP Customers** - Learn why they left (preventable churn insights)
4. **High-Growth ICP Customers** - Future product direction insights
5. **Activated Free Users** - Conversion insights

**PM Warning:** Don't over-index on non-ICP feedback. A hobbyist's feature request may not serve high-growth startups.

***

### What to Ask

**Jobs-to-Be-Done Framework:**

1. **"What were you trying to accomplish when you used [feature]?"**
2. **"What did you use before PostHog? Why did you switch?"**
3. **"What would make you 'very disappointed' if PostHog disappeared?"**
4. **"What's the biggest workflow friction you face with PostHog?"**
5. **"If you could add one feature, what would it be and why?"**

**PM Insight:** Ask about workflows, not features. Customers ask for features but what they need are solutions to workflow problems.

***

### How to Share Learnings

**PostHog Culture:** Asynchronous sharing via GitHub PR in product-internal repo

**PM Action:**
- Document findings after every interview
- Tag insights by ICP segment, product area, and theme
- Share in growth reviews and team standups
- Create "customer insight" PRs for engineering teams to read

***

## 12. PM SUCCESS FRAMEWORK

### Your First 30 Days

**Week 1:** Get stuck into execution
- Join team standups
- Arrange 2+ customer calls (via CS initially)
- Learn current projects
- Use PostHog to gather data supporting existing projects
- Share interesting finding in company all-hands

**PM Heuristic:** Don't try to change everything immediately. Support existing projects first, build credibility.

***

### Your First 90 Days

**Month 1:** Your teams hit goals faster
- Reduce scope and increase impact of big projects
- Give context for better solutions
- Remove bottlenecks

**PM Heuristic:** PMs are context providers and bottleneck removers, not roadmap dictators.

***

### Your First Quarter

**Quarter 1:** Hit goals and set next quarter strategy
- Pull out stops to help team hit goals
- Work with leadership to define ambitious next-quarter goals
- Use data and customer context to rationalize priorities

**PM Heuristic:** Set context through data and customer insights, let engineering teams decide "how."

***

### Long-Term Success Metrics

**PM Evaluation Criteria:**

1. **Growth Review Quality** - Are your monthly reviews insightful and actionable?
2. **Customer Interview Cadence** - Hitting 1/week target?
3. **Team Velocity** - Are engineering teams shipping faster with your context?
4. **Product Metrics** - Are your products hitting growth targets (9-20% MoM)?
5. **Blind Spot Elimination** - Did you research and document the "biggest unknowns"?
6. **Cross-Product Impact** - Are you performing company-level analytics beyond your team's scope?

***

## 13. ANTI-PATTERNS: What NOT to Do

### Anti-Pattern 1: Building for Non-ICP

**Mistake:** Customer from outside ICP requests feature, PM adds to roadmap.

**Why It's Wrong:** Dilutes product focus, doesn't serve core customers.

**PM Rule:** **Politely decline non-ICP feature requests.** Explain it's not in line with current product direction.

***

### Anti-Pattern 2: Roadmap Dictation

**Mistake:** PM creates detailed roadmap and assigns tasks to engineers.

**Why It's Wrong:** PostHog is product-minded engineering org - engineers own solutions.

**PM Rule:** Set context and let engineering teams decide what to build and how.

***

### Anti-Pattern 3: Ignoring Activation Data

**Mistake:** Focusing on new signups without tracking activation and retention.

**Why It's Wrong:** Vanity metric - signups don't equal revenue or PMF.

**PM Rule:** Track per-product activation religiously. If activation drops, sound the alarm.

***

### Anti-Pattern 4: Copying Competitors

**Mistake:** "Amplitude has this feature, we need it too."

**Why It's Wrong:** PostHog differentiates on integration and developer-friendliness, not feature parity.

**PM Rule:** Build features **your ICP** needs, not what competitors have. Compete on workflow consolidation, not feature lists.

***

### Anti-Pattern 5: Over-Optimizing for Current Scale

**Mistake:** Building features that only matter at 100M+ events/day.

**Why It's Wrong:** ICP is 15-500 employee startups, not Google-scale companies.

**PM Rule:** Optimize for ICP scale (1M-100M events/month), not hypothetical enterprise scale.

***

## 14. THE PM'S MENTAL CHECKLIST

**Before Every Decision, Ask:**

✅ **Does this serve our ICP?** (High-growth startups, 15-500 employees)

✅ **Does this improve activation or retention for activated users?**

✅ **Does this increase integration value across products?** (The moat is workflow consolidation)

✅ **Is this developer-friendly?** (Code-first, transparent, SQL-accessible)

✅ **Can we self-serve this?** (Or does it require sales-led motion?)

✅ **Will this make customers "very disappointed" if we removed it?** (PMF litmus test)

✅ **Have I validated this with 3+ customer interviews?**

✅ **Does this reduce context-switching for product teams?** (The ultimate value prop)

***

## 15. THE POSTHOG PM MANIFESTO

**Core Beliefs:**

1. **ICP Clarity is Everything** - Every decision flows from understanding who we build for

2. **Activation > Acquisition** - Better to have 1,000 activated users than 10,000 signups

3. **Integration is the Moat** - Competitors can copy features, but workflow consolidation is hard to replicate

4. **Developer Experience is a Competitive Advantage** - Technical buyers value transparency, SQL access, open source

5. **Customer Interviews are Non-Negotiable** - Data shows what happens, interviews show why

6. **Engineers Own Solutions** - PMs provide context, engineers decide what and how to build

7. **Free Tier is PMF Validation** - If free users don't activate and retain, paid won't either

8. **Multi-Product Usage = Success** - Customers using 3+ products have the highest retention

9. **Speed with Communication > Perfection** - ICP has high bug tolerance if we're responsive

10. **Context > Control** - Great PMs set context that enables autonomous teams to make great decisions

***

## CONCLUSION: The PM's North Star

**At PostHog, PMs succeed by becoming the team's "intelligence officer"**—providing:

- **Market Intelligence:** Competitive landscape, industry trends
- **Customer Intelligence:** Jobs-to-be-done, pain points, delighters
- **Product Intelligence:** Usage patterns, activation/retention data, growth metrics
- **Strategic Intelligence:** Where to focus, what to deprioritize, ICP alignment

**Your job is NOT to control the roadmap. Your job is to make engineering teams so well-informed that they build the right things, faster.**

**The PM who can say "Here's what customers need, here's what the data shows, here's what competitors are doing, here's where we should focus"—and then get out of the way—will thrive at PostHog.**

***

**Remember:** PostHog's success comes from building the ultimate workflow tool for product engineers at high-growth startups. Every PM decision should ladder up to that vision.
