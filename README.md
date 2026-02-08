# Claude Code Skills Collection

A curated collection of specialized skills for [Claude Code](https://github.com/anthropics/claude-code) - Anthropic's official CLI for Claude.

## What Are Skills?

Skills are packaged prompts and resources that extend Claude Code's capabilities with specialized domain expertise. Each `.skill` file contains structured instructions, frameworks, and reference materials that transform Claude into a domain expert.

## Installation

### Method 1: Clone Repository (Recommended)
```bash
git clone https://github.com/onatvural/Claude-Skills.git ~/.claude/skills
```

### Method 2: Download Individual Skills
Download the `.skill` file and place it in your `~/.claude/skills/` directory.

### Activation
Skills are automatically available in Claude Code. Invoke them based on their trigger patterns or explicitly reference the skill name.

---

## Available Skills

### 1. Warren Buffett Analyst
**File:** `warren-buffett-analyst.skill`

Value investing analysis using Warren Buffett's proven methodology. Transforms Claude into the Oracle of Omaha with his folksy Midwestern wisdom.

**Capabilities:**
- Owner Earnings calculation
- Intrinsic value DCF analysis
- Moat classification (inevitable/formidable/strong/questionable)
- Position sizing with modified Kelly Criterion
- Margin of safety analysis
- Buffett Indicator for market timing

**Trigger Patterns:**
- Stock valuation requests
- Competitive moat assessment
- Business quality evaluation
- Investment decision analysis
- "Is this a good investment?"

**Example Prompts:**
```
"Analyze Apple's competitive moat using Buffett's framework"
"Calculate owner earnings for Microsoft"
"What would Buffett think of this business model?"
"Is the market overvalued right now?"
```

---

### 2. Global Macro-Political Analyst
**File:** `global-macro-analyst.skill`

Geopolitical and macroeconomic analysis for understanding global events and their investment implications. Transforms Claude into a battle-hardened geopolitical strategist.

**Capabilities:**
- Decode geopolitical events (wars, sanctions, trade wars)
- Great power competition analysis (US-China-Russia dynamics)
- Risk scenario building with probability weights
- PESTEL country/region analysis
- Game theory for strategic moves
- Economic constraints analysis (Impossible Trinity, Fiscal Space)
- Sanctions and trade war escalation assessment
- Hybrid warfare and deterrence analysis

**Included Frameworks:**
| Category | Frameworks |
|----------|------------|
| Strategic Environment | PESTEL, Levels of Analysis, Great Power Matrix |
| Actor Behavior | Game Theory, Two-Level Game, Regime Stability |
| Economic Constraints | Impossible Trinity, Fiscal Space, CB Credibility |
| Risk & Vulnerability | Country Risk, Supply Chain, Contagion |
| Conflict & Coercion | Sanctions, Trade War, Hybrid Warfare, Deterrence |
| Scenario & Decision | Scenario Planning, Alliance Reliability, Decision Synthesis |

**Trigger Patterns:**
- International conflicts and territorial disputes
- Great power competition questions
- Energy/commodity market analysis
- Currency movements and sanctions
- "What happens now?" questions
- "How will X affect markets?"
- Scenario analysis requests

**Example Prompts:**
```
"What are the implications of rising US-China tensions for semiconductor supply chains?"
"Analyze the oil market impact if sanctions on Iran are lifted"
"Build scenarios for the Taiwan situation"
"How does the Russia-Ukraine conflict affect European energy security?"
"What's Turkey's economic outlook given its impossible trinity constraints?"
```

---

## Skill File Structure

Each `.skill` file is a ZIP archive containing:

```
skill-name/
├── SKILL.md              # Main skill definition and instructions
├── scripts/              # Optional Python/JS helper scripts
├── references/           # Reference documents and frameworks
│   ├── frameworks/       # Analysis frameworks
│   └── *.md             # Supporting documentation
└── assets/              # Templates, examples, case studies
```

## Creating Your Own Skills

1. Create a directory with your skill name
2. Add a `SKILL.md` with frontmatter:
   ```yaml
   ---
   name: your-skill-name
   description: Brief description and trigger patterns
   ---
   ```
3. Add any supporting files (scripts, references, assets)
4. Package as ZIP: `zip -r your-skill-name.skill your-skill-name/`

## Contributing

Contributions welcome! Please:
1. Fork the repository
2. Add your skill following the structure above
3. Update this README with skill documentation
4. Submit a pull request

## License

MIT License - See [LICENSE](LICENSE) for details.

## Disclaimer

These skills are designed for educational and analytical purposes. Investment analysis skills do not constitute financial advice. Always consult qualified professionals before making investment decisions.

---

**Created by:** [@onatvural](https://github.com/onatvural)
