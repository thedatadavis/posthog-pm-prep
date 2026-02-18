# VelocityGrid: PM Impact Tracker
View live demo: https://vel.pgpln.app

The VelocityGrid is a visual diagnostic tool designed to map the "health" of a product team's output. Unlike a Jira backlog or a Gantt chart—which track *what* is being done and *when*—this tool tracks *value* and *efficiency*.

It answers the two most critical questions in product management:

1. **Did it matter?** (Impact)
2. **Was it hard?** (Speed/Velocity)

## 1. The Geometry of Shipping

The grid is divided into a Cartesian coordinate system where every shipped feature is a data point.

### The Axes

* **Y-Axis (Vertical): Impact Score (1–10)**
  * **Definition:** The tangible value delivered to the user or the business.
  * **10 (Top):** Game-changer. Significantly moves a KPI (revenue, retention, conversion).
  * **1 (Bottom):** Negligible. A typo fix, a minor UI tweak, or a feature nobody used.


* **X-Axis (Horizontal): Speed Score (1–10)**
  * **Definition:** The velocity of execution. This is the inverse of "Effort/Friction."
  * **10 (Right):** Lightning fast. Shipped in hours or days with zero friction.
  * **1 (Left):** A slog. Took months, required massive refactoring, or got stuck in "dependency hell."



### The Four Quadrants

Where a dot lands tells the story of that feature.

| Quadrant | Location | Nickname | Implication |
| --- | --- | --- | --- |
| **I** | **Top-Right** | **The Flow State** | **High Value / Low Friction.** This is the ideal. The team understands the code, the scope is clear, and the customer gets value. |
| **II** | **Top-Left** | **The Slog** | **High Value / High Friction.** These are necessary evils (e.g., major refactors, complex compliance features). Acceptable occasionally, but dangerous if it becomes the norm. |
| **III** | **Bottom-Right** | **Snacks** | **Low Value / Low Friction.** "Quick wins" or "low-hanging fruit." These feel good to ship but don't build a business. Beware of becoming a "Feature Factory" that ships 100 things that don't matter. |
| **IV** | **Bottom-Left** | **The Danger Zone** | **Low Value / High Friction.** The morale killer. You spent weeks on something that users don't care about. These projects should have been killed in the discovery phase. |

## 2. The Time Dimension (Temporal Fading)

Static charts lie because they treat a feature shipped a year ago the same as a feature shipped today. VelocityGrid uses **color opacity** to represent time.

* **Green (Solid):** Shipped in the last 14 days. This is your current reality.
* **Blue (50% Opacity):** Shipped 15–30 days ago. The recent past.
* **Gray (15% Opacity):** Shipped 30+ days ago. Historical context.

**Why this matters:**
This creates a "comet tail" effect. You can visually see the trajectory of the team. If the gray dots (history) are in the Top-Right, but the green dots (current) are in the Bottom-Left, your team is degrading. You are moving slower and building less valuable things than you used to.

## 3. Diagnosing Team Health

Use the visual patterns to diagnose systemic issues.

### Scenario A: The Leftward Drift (Tech Debt)

* **Visual:** Older dots (gray) are on the right. Newer dots (green) are clustering on the left.
* **Diagnosis:** The codebase is rotting. Features that used to take 2 days now take 2 weeks because of spaghetti code or lack of testing.
* **Action:** Pause feature work. Invest in refactoring and CI/CD.

### Scenario B: The Bottom-Right Trap (The Feature Factory)

* **Visual:** A massive cluster of dots in the Bottom-Right. High speed, low impact.
* **Diagnosis:** The team is optimizing for "output," not "outcome." You are shipping fast, but you aren't solving hard problems. This often happens when teams are measured by the *number* of tickets closed rather than business results.
* **Action:** Revisit the product strategy. Focus on fewer, deeper problems.

### Scenario C: The Scattershot (No Strategy)

* **Visual:** Dots are evenly distributed across the entire board with no pattern.
* **Diagnosis:** The team lacks a unified direction. You are indiscriminately picking up "Slogs," "Snacks," and "Big Bets" without prioritization criteria.
* **Action:** Implement stricter prioritization frameworks (e.g., RICE scoring) before a ticket enters development.

### Scenario D: The Bottom-Left Anchor

* **Visual:** Consistent clustering in the low-speed, low-impact zone.
* **Diagnosis:** This is a failure of **Product Discovery**. The team is building things that are harder than expected and less valuable than predicted.
* **Action:** Improve technical scoping (engineering estimation) and customer validation (design research) before writing code.
