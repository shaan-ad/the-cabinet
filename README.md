# The Cabinet

> 26 AI executive personas for Claude Code and Cowork. Every leader needs a cabinet.

Point any decision, strategy, or problem at The Cabinet and get perspectives from every leadership angle. A CEO who challenges your vision. A CFO who demands the numbers. A Reality Checker who tears apart your assumptions.

Pure markdown. Zero code. Install in one command.

## Install

### Claude Code (CLI)

```bash
claude plugin marketplace add shaan-ad/the-cabinet
claude plugin install the-cabinet@the-cabinet
```

### Claude Cowork (Desktop / Web)

1. [Download the plugin zip](https://github.com/shaan-ad/the-cabinet/archive/refs/heads/main.zip)
2. In Cowork, go to **Customize** > **+** next to Personal plugins
3. Select **Create plugin** > **Upload plugin**
4. Upload the zip file

### VS Code / JetBrains

Type `/plugins` in the Claude Code panel, add `shaan-ad/the-cabinet` as a marketplace source, then install from the GUI.

### No plugin system? Just use the markdown.

Every persona is a standalone `.md` file. Open any file in `cabinet/`, `startup/`, or `advisors/`, copy the content, and paste it as a system prompt in ChatGPT, Gemini, Cowork, or any AI tool.

---

## The Leadership Cabinet

C-suite executives for strategic decisions.

| | Persona | Role | Lens |
|---|---------|------|------|
| :chess_pawn: | **[The CEO](cabinet/ceo.md)** | Chief Executive | Vision, strategy, stakeholder management |
| :bar_chart: | **[The CFO](cabinet/cfo.md)** | Chief Financial | Unit economics, burn rate, ROI |
| :gear: | **[The CTO](cabinet/cto.md)** | Chief Technology | Architecture, tech debt, build vs buy |
| :loudspeaker: | **[The CMO](cabinet/cmo.md)** | Chief Marketing | Brand, positioning, GTM |
| :factory: | **[The COO](cabinet/coo.md)** | Chief Operations | Process, scale, efficiency |
| :dart: | **[The CPO](cabinet/cpo.md)** | Chief Product | User value, prioritization, roadmap |
| :people_holding_hands: | **[The CHRO](cabinet/chro.md)** | Chief People | Culture, hiring, org design |
| :balance_scale: | **[The General Counsel](cabinet/general-counsel.md)** | Legal | Risk, compliance, IP, contracts |
| :clipboard: | **[The Chief of Staff](cabinet/chief-of-staff.md)** | Execution | Alignment, communication, follow-through |
| :classical_building: | **[The Board Advisor](cabinet/board-advisor.md)** | Governance | Fiduciary duty, long-term value |

## The Startup Team

Scrappy, opinionated team for early-stage companies.

| | Persona | Role | Lens |
|---|---------|------|------|
| :hammer_and_wrench: | **[The Technical Cofounder](startup/technical-cofounder.md)** | Engineering | MVP scope, tech stack, shipping speed |
| :rocket: | **[The Growth Lead](startup/growth-lead.md)** | Acquisition | Channels, CAC, viral loops |
| :money_with_wings: | **[The Investor Relations](startup/investor-relations.md)** | Fundraising | Pitch, metrics, term sheets |
| :scroll: | **[The Startup Lawyer](startup/startup-lawyer.md)** | Legal | Incorporation, IP, contracts |
| :art: | **[The Product Designer](startup/product-designer.md)** | UX/Design | User flows, simplicity, usability |
| :handshake: | **[The Customer Success](startup/customer-success.md)** | Retention | Onboarding, churn, NPS |
| :mag: | **[The Data Analyst](startup/data-analyst.md)** | Metrics | Dashboards, cohorts, experimentation |
| :writing_hand: | **[The Content Strategist](startup/content-strategist.md)** | Brand | Story, positioning, thought leadership |
| :shield: | **[The DevOps Lead](startup/devops-lead.md)** | Infrastructure | CI/CD, monitoring, launch readiness |
| :crystal_ball: | **[The Angel Investor](startup/angel-investor.md)** | Advisory | Market timing, competition, patterns |

## The Advisors

External specialists who bring outside perspective.

| | Persona | Role | Lens |
|---|---------|------|------|
| :briefcase: | **[The VC Partner](advisors/vc-partner.md)** | Investment | Market size, defensibility, venture-scale |
| :mirror: | **[The Executive Coach](advisors/executive-coach.md)** | Leadership | Self-awareness, delegation, growth |
| :fire_extinguisher: | **[The Crisis Manager](advisors/crisis-manager.md)** | Risk | Scenario planning, worst-case prep |
| :bank: | **[The M&A Advisor](advisors/ma-advisor.md)** | Corporate Dev | Valuation, synergies, build/buy/partner |
| :robot: | **[The AI Strategist](advisors/ai-strategist.md)** | Technology | AI adoption, use cases, implementation |
| :no_entry_sign: | **[The Reality Checker](advisors/reality-checker.md)** | Devil's Advocate | Assumptions, blind spots, cognitive biases |

---

## Usage

### Ask a specific persona

```
Run this pricing strategy past the CFO
```

### Get a team perspective

```
I need the Startup Team to review my pitch deck
```

### Convene the full cabinet

```
Get me the full cabinet's take on this acquisition opportunity
```

### Challenge your thinking

```
What would the Reality Checker say about our Q3 plan?
```

---

## What Makes This Different

| | Generic Prompts | Prompt Libraries | The Cabinet |
|---|---|---|---|
| **Depth** | Surface-level | Template-based | 800+ words per persona with real frameworks |
| **Perspective** | One voice | Multiple styles | Distinct decision frameworks per role |
| **Challenge** | Agrees with you | Follows instructions | Pushes back on blind spots |
| **Expertise** | Generalist | Role-aware | Named frameworks (DCF, Porter's Five Forces, Kano Model, etc.) |

## By the Numbers

- **26** specialized executive personas
- **3** teams (Cabinet, Startup, Advisors)
- **180+** signature questions that expose blind spots
- **50+** named decision frameworks
- **0** lines of code (pure markdown)

---

## How Each Persona Is Built

Every persona includes:

- **Personality**: Communication style, temperament, priorities
- **Core Mission**: Primary responsibilities with clear deliverables
- **Decision Framework**: Real named frameworks specific to the role
- **Questions They Always Ask**: Sharp questions that expose blind spots
- **What They Push Back On**: Triggers for skepticism and challenge
- **Communication Style**: Quoted example phrases showing their voice
- **How to Use**: Example prompts for Claude Code

---

## Contributing

Want to add a persona? Follow this format:

1. Pick a role that is missing from the current roster
2. Create a `.md` file in the appropriate team directory
3. Follow the [persona template](CONTRIBUTING.md) (frontmatter + 6 sections)
4. Make it genuinely distinct from existing personas
5. Submit a PR

---

## License

MIT

---

<div align="center">

Built by [Shaan Agara](https://www.linkedin.com/in/shaan-agara/) | Also check out [PM-OS](https://github.com/shaan-ad/pm-os)

</div>
