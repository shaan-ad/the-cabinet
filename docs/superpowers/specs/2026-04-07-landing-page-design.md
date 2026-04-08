# The Cabinet: Landing Page Design Spec

## Overview

A single self-contained HTML file that showcases The Cabinet (26 AI executive personas for Claude Code) and drives installation. Bold editorial visual style: dark backgrounds, purple/pink gradients, oversized sans-serif type, animated elements.

**Goal:** Equal weight on understanding the product and converting to install.

**Tech:** Single `index.html` with inline CSS and JS. One external asset (`assets/headshot.jpg`). Zero dependencies. GitHub Pages ready. Responsive.

---

## Sections

### 1. Hero

Full-viewport section with animated radial gradient background (purple and pink on dark #0a0a0a base).

Content:
- "The Cabinet" in ~64px, font-weight 800, gradient text (white to light purple)
- Tagline: "26 AI executive personas for Claude Code. Every leader needs a cabinet."
- Install command box (2-step, following PM-OS format):
  - Step 1: `claude plugin marketplace add shaan-ad/the-cabinet` (copy-to-clipboard)
  - Step 2: `claude plugin install the-cabinet` (copy-to-clipboard)
- Stats bar: 26 personas | 180+ questions | 50+ frameworks | 0 lines of code

Animation: Slow drifting radial gradient in the background (CSS keyframes, subtle).

### 2. What is The Cabinet?

Short explainer section. 2-3 sentences pulled from README:

"Point any decision, strategy, or problem at The Cabinet and get perspectives from every leadership angle. A CEO who challenges your vision. A CFO who demands the numbers. A Reality Checker who tears apart your assumptions. Pure markdown. Zero code. Install in one command."

### 3. Persona Grid

The core section. Three tabs for the three teams:

**Tab names:**
- Executives Leadership (10 personas)
- Startup Cabinet (10 personas)
- Startup Advisors (6 personas)

**Card design (collapsed):**
- Subtle monochrome icon (single muted color, consistent style across all 26 personas, not colorful emoji). Use thin-line SVG icons in a muted purple/gray tone.
- Persona name (bold)
- Role title (smaller, muted purple)
- Lens description (1-2 lines, gray)
- 2 signature questions (styled as quotes, light purple)

**Card design (expanded, on click):**
- Everything from collapsed state
- Frameworks section: displayed as pill-shaped tags
- "What they push back on" (1-2 lines)
- Example prompt in a dark code-style box

Cards use CSS transitions for smooth expand/collapse. Only one card expanded at a time (accordion behavior).

**Persona data:**

#### Executives Leadership

| # | Icon concept | Name | Role | Lens | Question 1 | Question 2 | Frameworks | Pushes back on |
|---|---|---|---|---|---|---|---|---|
| 1 | strategy/chess | The CEO | Chief Executive | Vision, strategy, stakeholder alignment | "What would have to be true for this to be a good idea?" | "If we say yes to this, what are we saying no to?" | Porter's Five Forces, 2x2 prioritization | Consensus-seeking, strategy with no trade-offs, vanity metrics |
| 2 | chart/finance | The CFO | Chief Financial | Unit economics, runway, payback periods | "What's the fully-loaded cost, including people-hours?" | "If this takes twice as long and costs 50% more, do we still do it?" | Three-scenario modeling, ROI ranking | Hockey-stick projections, conflating revenue with cash |
| 3 | gear/tech | The CTO | Chief Technology | Systems thinking, tech debt, build vs buy | "What's the blast radius if this fails?" | "Is this essential complexity, or accidental?" | Three Horizons of Regret, Boring Technology | Resume-driven development, rewrites without business case |
| 4 | megaphone/marketing | The CMO | Chief Marketing | Positioning, demand gen, buyer psychology | "Who is the buyer, and what trigger makes them look?" | "What do we want the market to believe that they don't?" | Dunford positioning, Byron Sharp | Feature-led messaging, launching without clear ICP |
| 5 | process/operations | The COO | Chief Operations | Bottlenecks, handoffs, capacity analysis | "Who owns the handoff between these two teams?" | "If we doubled volume tomorrow, which process breaks first?" | Theory of Constraints, Process-People-Tools | Adding headcount before fixing the process |
| 6 | target/product | The CPO | Chief Product | User problems, prioritization, continuous PMF | "What user problem are we solving, and how do we know it's real?" | "What's the smallest version that lets us learn?" | Modified RICE, Opportunity Solution Tree, Kano | Solutions disguised as problems, skipping discovery |
| 7 | people/culture | The CHRO | Chief People | Org health, hiring quality, retention signals | "If this person left tomorrow, what would break?" | "Are we hiring for the role we need in 12 months?" | Lencioni's Five Dysfunctions, "Who" scorecards | Hiring for speed over quality, culture as perks |
| 8 | scale/legal | General Counsel | Legal | Risk translation, contracts, IP, compliance | "If this goes wrong, what's the worst-case financial exposure?" | "What precedent does this set?" | Probability-impact matrix, contract position tiers | Verbal agreements, skipping legal to move fast |
| 9 | link/alignment | Chief of Staff | Execution | Decision hygiene, cross-functional gaps, follow-through | "Has this decision been communicated to people who need to act?" | "Are we aligned, or are we just being polite?" | Five-point decision docs, meeting taxonomy | Meetings without agendas, action items without owners |
| 10 | building/governance | Board Advisor | Governance | Promises vs performance, capital allocation, risk oversight | "If I were an outside investor, what would concern me?" | "Which assumption, if wrong, most changes the outcome?" | Promises vs performance, Buffett capital allocation | Narrative drift, vanity metrics in board decks |

#### Startup Cabinet

| # | Icon concept | Name | Role | Lens | Question 1 | Question 2 | Frameworks | Pushes back on |
|---|---|---|---|---|---|---|---|---|
| 1 | wrench/engineering | Technical Cofounder | Engineering | MVP scope, shipping cadence, reversibility | "If we had to ship by Friday, what would we cut?" | "Is this a reversible or irreversible decision?" | Reversibility Test, Boring Technology | Microservices before PMF, custom infra before Series A |
| 2 | trending/growth | Growth Lead | Acquisition | CAC/payback, activation, cohort retention | "What's our activation metric, and what % hit it in first session?" | "Which channel brought our best-retained users?" | ICE framework, Bullseye Framework | "We need more traffic" before fixing conversion |
| 3 | money/fundraising | Investor Relations | Fundraising | Readiness, term sheets, milestone-driven raises | "What milestone will this capital help you reach?" | "What metric in your deck makes an investor lean forward?" | Three Pillars readiness test, tiered targeting | Raising too early, valuation obsession |
| 4 | document/legal | Startup Lawyer | Legal | Severity vs reversibility, cap tables, IP, vesting | "Do you have signed IP assignment from everyone who wrote code?" | "What is your co-founder vesting schedule?" | Severity vs Reversibility matrix, Slicing Pie | Handshake agreements, 50/50 splits without vesting |
| 5 | layout/design | Product Designer | UX/Design | Time-to-value, progressive disclosure, one job per screen | "What is the user trying to accomplish, in one sentence?" | "What happens if we remove this element?" | Nielsen's heuristics, Five-Second Test, Fitts's Law | Feature additions that compromise clarity, "Make it pop" |
| 6 | heart/retention | Customer Success | Retention | Onboarding, health scoring, time-to-value, churn | "What does 'success' look like for this customer?" | "Which customers are going quiet?" | Health Score model, "First Value" framework | Treating CS as support, adding features before checking adoption |
| 7 | bar-chart/metrics | Data Analyst | Metrics | North Star hierarchy, cohort vs aggregate, statistical rigor | "What decision will this metric help you make?" | "Are we looking at cohort view or aggregate?" | Metrics Hierarchy, "Glanceable, Explorable, Actionable" | Averages without distributions, calling A/B tests early |
| 8 | pen/content | Content Strategist | Brand | Unique POV, founder voice, distribution over creation | "What does this company believe that competitors do not?" | "Could I tell which company this is with the logo hidden?" | POV Audit, "Obviously Awesome," 1-to-7 distribution | Generic content any competitor could publish |
| 9 | server/infrastructure | DevOps Lead | Infrastructure | Operational burden, managed services first, progressive delivery | "What is our rollback plan if this deployment breaks?" | "If we get 10x traffic tomorrow, what breaks first?" | Operational Burden, Managed Services First, Three Pillars | Kubernetes before 10 engineers, "We will add monitoring later" |
| 10 | eye/advisory | Angel Investor | Advisory | Founder-market fit, timing, market structure, pull signals | "What is the contrarian belief embedded in this company?" | "If a competitor copied your product, what would you still have?" | Founder-Market Fit + Timing, "Kill the Company" | "We have no competition," top-down TAM slides |

#### Startup Advisors

| # | Icon concept | Name | Role | Lens | Question 1 | Question 2 | Frameworks | Pushes back on |
|---|---|---|---|---|---|---|---|---|
| 1 | shark/venture | VC Partner | Investment | Power Law, bottom-up TAM, defensibility, burn multiples | "Walk me through the TAM bottom-up." | "Which of Helmer's 7 Powers do you have today?" | Rachleff market-team, Helmer 7 Powers | Top-down TAM, defensibility via "execution" |
| 2 | mirror/coaching | Executive Coach | Leadership | Avoidance patterns, identity tasks, delegation bottlenecks | "What conversation have you been putting off?" | "You describe this as a team problem. What if it's a you problem?" | Kegan's adult development, Johari Window | Blaming the team for leadership problems |
| 3 | alert/crisis | Crisis Manager | Risk | Pre-mortem, communication speed, single points of failure | "If this goes wrong, what does the headline look like?" | "Who owns crisis communication right now?" | Cynefin framework, Shell scenario methodology | "That will never happen to us," untested crisis plans |
| 4 | handshake/deals | M&A Advisor | Corporate Dev | Build vs buy time-value, synergy rates, deal structure | "If you could not acquire this, what would it cost to build?" | "Walk me through the synergy math line by line." | Valuation triangulation, synergy haircuts | "Strategic premium" justifying overpayment |
| 5 | brain/ai | AI Strategist | Technology | Business impact vs feasibility, data readiness, build vs buy AI | "What business metric will this AI project move, and by how much?" | "Is this a moat or a wrapper any competitor could replicate?" | 2x2 impact/feasibility, AI readiness dimensions | "AI-first" without use cases, demo-driven development |
| 6 | skull/challenge | Reality Checker | Devil's Advocate | Epistemic rigor, cognitive bias, evidence vs narrative | "What would have to be true for this to fail?" | "Strip the narrative. What raw data points does this plan rest on?" | Epistemic rigor hierarchy, "Steel man then destroy" | Consensus without dissent, best-case assumptions |

### 4. How It Works

Three-step visual layout:

1. **Install** - Copy-paste one command. Show the install command box again.
2. **Ask** - Example prompts: "Run this pricing strategy past the CFO", "I need the Startup Team to review my pitch deck", "What would the Reality Checker say about our Q3 plan?"
3. **Get Perspective** - The persona challenges your thinking with their specific frameworks and questions.

Below the 3-step visual: tabbed install instructions for:
- Claude Code (CLI)
- Claude Cowork (Desktop/Web)
- VS Code / JetBrains
- Raw markdown (no plugin system)

### 5. What Makes This Different

Comparison table with 4 rows. The Cabinet column visually highlighted (purple border or background).

|  | Generic Prompts | Prompt Libraries | The Cabinet |
|---|---|---|---|
| Depth | Surface-level | Template-based | 800+ words per persona with real frameworks |
| Perspective | One voice | Multiple styles | Distinct decision frameworks per role |
| Challenge | Agrees with you | Follows instructions | Pushes back on blind spots |
| Expertise | Generalist | Role-aware | Named frameworks (DCF, Porter's, Kano, etc.) |

### 6. Footer

- Circular headshot of Shaan Agara (loaded from `assets/headshot.jpg`) next to "Built by Shaan Agara" with LinkedIn link
- GitHub repo link
- "Also check out PM-OS" cross-link
- Minimal, same dark theme

---

## Visual Design System

**Colors:**
- Background: #0a0a0a (base), #1a1a1a (cards/sections)
- Text: #e2e8f0 (primary), #9ca3af (secondary), #6b7280 (tertiary)
- Accent: #7c3aed (purple primary), #a78bfa (purple light), #c4b5fd (purple pale)
- Gradient: purple (#7c3aed) to pink (#ec4899) for background effects
- Highlight: rgba(139,92,246,0.1) for card hovers and active states

**Typography:**
- Font: system-ui, -apple-system, sans-serif
- Hero title: 64px, weight 800, letter-spacing -2px
- Section titles: 36px, weight 800, letter-spacing -1px
- Body: 16px
- Code/install: SF Mono, Fira Code, monospace

**Icons:**
- Consistent monochrome SVG icons for all 26 personas
- Single color: muted purple (#a78bfa) or gray (#6b7280)
- Thin-line style, same visual weight across all icons
- No colorful emoji

**Interactions:**
- Card hover: slight lift (translateY -2px), purple border glow
- Card click: smooth expand with CSS transition (~300ms)
- Tab switching: instant content swap
- Install box: hover highlight, click copies to clipboard with feedback text
- Background gradient: slow drift animation (8s ease-in-out)

**Responsive:**
- Desktop: 3-column card grid
- Tablet: 2-column card grid
- Mobile: single column, full-width cards

---

## File Structure

```
the-cabinet/
  index.html          # The landing page (new)
  assets/
    headshot.jpg       # Author headshot (new)
```

---

## Data Source

All persona content is pulled directly from the markdown files in `cabinet/`, `startup/`, and `advisors/`. The landing page hardcodes this content in HTML (not dynamically loaded) since it is a static single-file page.

---

## Out of Scope

- No JavaScript framework or build step
- No dynamic markdown parsing at runtime
- No analytics or tracking
- No dark/light mode toggle (dark only)
- No search or filtering within the persona grid
- No backend
