---
name: mirofish-simulation
description: AI multi-agent simulation engine for scenario prediction and decision rehearsal. Spawns personas with distinct incentives, biases, and memory to simulate social dynamics over multiple rounds. Use when analyzing campaign outcomes, policy impacts, market reactions, PR crisis scenarios, or any multiplayer situation where human behavior is the key variable. Triggers: "simulate scenario", "predict outcome", "decision rehearsal", "campaign pressure test", "multi-agent analysis", "stakeholder simulation", "what-if analysis", "scenario planning".
license: MIT
compatibility: Web browser, any MCP-compatible agent via API
metadata:
  author: 666ghj
  version: "1.0"
  url: https://mirofish.homes
---

# MiroFish — AI Simulation Chat for Scenario Prediction

MiroFish is an open-source AI simulation engine that rehearses the future by spawning personas with distinct incentives, biases, and memory, then letting them interact across social surfaces over multiple rounds. Unlike single-model Q&A, it produces emergent dynamics you can't script.

> **Live at**: [mirofish.homes](https://mirofish.homes/)  
> **Source**: [github.com/666ghj/MiroFish](https://github.com/666ghj/MiroFish)

## When to Use This Skill

- **Campaign pressure testing** — how will different audiences amplify, resist, or reinterpret a message?
- **Policy impact analysis** — which stakeholders react first, and how does the cascade unfold?
- **Market reaction modeling** — simulate competitor responses before real-world deployment
- **PR crisis rehearsal** — identify the persona that triggers the first negative cascade
- **Product launch scenarios** — test positioning against multiple buyer personas simultaneously
- **Counterfactual exploration** — "What if we changed this one variable?"

## When Not to Use

- Simple factual Q&A (use standard LLM chat)
- Single-perspective analysis where interaction dynamics don't matter
- Real-time data analysis requiring live API feeds

## How It Works

### The Five-Stage Creative Process

1. **Seed the world**  
   Describe the scenario in plain language. Attach a strategy memo, policy brief, or market note for grounding. No structured input required — just like briefing a team.

2. **Map the dynamics**  
   The engine extracts actors, relationships, pressures, and factual anchors into a knowledge graph — the cast and conflict map before simulation begins.

3. **Run the rehearsal**  
   AI personas — each with distinct incentives, biases, and memory — interact across social surfaces over multiple rounds. Personas respond to each other, not just the initial prompt, producing emergent dynamics.

4. **Read the report**  
   A structured result card surfaces:
   - Most likely trajectory with confidence indicators
   - Risk signals and early warning flags
   - Narrative path analysis
   - Natural follow-up questions

5. **Keep directing**  
   Unlike a static forecast, continue questioning the simulation. Change variables. Test counterfactuals. Explore the world you created.

### Technical Architecture

| Component | Technology |
|-----------|-----------|
| Multi-agent orchestration | Custom persona spawning with memory persistence |
| Knowledge extraction | Graph-based actor/relationship mapping |
| Interaction surface | Chat interface with round-based progression |
| Deployment | Web application at [mirofish.homes](https://mirofish.homes/) |

## Inputs

| Input | Required | Description |
|-------|----------|-------------|
| Scenario description | Yes | Plain-language description of the situation to simulate |
| Supporting documents | No | Strategy briefs, policy documents, or market notes for factual grounding |
| Persona definitions | No | Custom stakeholder profiles (defaults to auto-generated) |

## Outputs

| Output | Description |
|--------|-------------|
| Trajectory forecast | Most likely outcome path with confidence score |
| Risk signals | Early warning indicators ranked by severity |
| Narrative paths | How different stakeholder narratives evolve over rounds |
| Follow-up questions | AI-generated deep-dive prompts for further exploration |

## Installation

### Web Access
Visit [mirofish.homes](https://mirofish.homes/) — no installation required.

### Self-Hosted (Open Source)
```bash
git clone https://github.com/666ghj/MiroFish.git
cd MiroFish
# Follow setup instructions in README
```

## Examples

### Example 1: Product Launch Scenario
```
Input: "We're launching a premium-priced AI writing tool. 
How will freelance writers, content agencies, and enterprise teams react?"

Output:
- Freelance writers: Price resistance → demand for free tier
- Content agencies: Cautious adoption → ROI comparison with alternatives
- Enterprise: Compliance concerns → security audit requests
- Risk signal: Freelancer backlash on social media within first 48 hours
```

### Example 2: Policy Change
```
Input: "Our platform is changing from free to freemium. 
How will our 50K existing users respond?"

Output:
- Power users: Mixed — some upgrade, some migrate
- Casual users: Majority churn unless retention hooks are strong
- Risk signal: Vocal minority organizing migration campaigns
- Recommendation: Phased rollout with grandfather clause for early adopters
```

## Validation

- [ ] Simulation completes with 3+ interacting personas
- [ ] Result card includes trajectory, risk signals, and follow-up questions
- [ ] Counterfactual queries produce meaningfully different outcomes
- [ ] Knowledge graph correctly maps actors and relationships

## Common Pitfalls

| Pitfall | Solution |
|---------|----------|
| Too few personas | Include at least 3 stakeholder types with conflicting interests |
| Vague scenario | Add specific constraints: timeline, budget, existing commitments |
| Ignoring counterfactuals | Always test at least one alternative variable |

## References

- [Live Application](https://mirofish.homes/)
- [GitHub Repository](https://github.com/666ghj/MiroFish)
- [Design Case Study](https://mirofish.homes/)
