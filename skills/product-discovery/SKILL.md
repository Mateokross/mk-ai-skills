---
name: product-discovery
description: "Run a full product discovery cycle on a product or feature idea: brainstorm ideas, surface risky assumptions, prioritize them, and design experiments, pausing for the user to choose at each checkpoint. Ends with a discovery plan. Use when the user wants to run discovery end to end, validate an idea before building it, or asks for a discovery plan."
---

# Product Discovery Cycle

Move from divergent thinking to focused validation in one structured workflow. This skill chains the brainstorm, assumption and experiment skills into an end-to-end process. It takes 15-30 minutes; tell the user that upfront.

## Workflow

### Step 1: Understand the discovery context

Decide whether this is:
- **Existing product**: continuous discovery on a known product with real users
- **New product**: initial discovery for a concept without validated demand

Ask the user, unless they already said:
- What are you exploring? (product idea, feature area, opportunity space)
- What do you already know? (prior research, customer feedback, data)
- What decision will this discovery inform? (build/kill, prioritize, pivot)

Read any files or links they provide (research, PRDs, transcripts, data) and pull insights from them before brainstorming.

### Step 2: Brainstorm ideas (divergent)

Apply the **brainstorm-ideas-existing** or **brainstorm-ideas-new** skill:
- Generate ideas from product manager, designer and engineer perspectives
- Present the top 10 ideas with a brief rationale each

**Checkpoint:** "Here are 10 ideas. Which ones should we stress-test? Pick 3-5, or I can carry all of them forward."

### Step 3: Identify assumptions (critical thinking)

For each selected idea, apply the **identify-assumptions-existing** or **identify-assumptions-new** skill:
- Surface assumptions across risk categories: Value (will users want it?), Usability (can they figure it out?), Feasibility (can we build it?), Viability (does the business case work?), and for new products Go-to-Market (can we reach and convert users?)
- Argue against each idea from several perspectives
- Compile one master list of assumptions across all ideas

### Step 4: Prioritize assumptions (focus)

Apply the **prioritize-assumptions** skill:
- Map assumptions on an Impact × Risk matrix
- Identify the leap-of-faith assumptions: high impact, high uncertainty
- Rank them by test priority, and group related assumptions that one test can cover

**Checkpoint:** "Here are your riskiest assumptions. Which ones feel most critical to validate first?"

### Step 5: Design experiments (validation)

For the top-priority assumptions, apply the **brainstorm-experiments-existing** or **brainstorm-experiments-new** skill:
- Design 1-2 experiments per critical assumption
- Existing products: A/B tests, fake doors, prototypes, user tests, data analysis
- New products: XYZ hypotheses, pretotypes, landing pages, concierge MVPs
- Give each one success criteria, timeline and effort
- Sequence experiments by dependency and effort

### Step 6: Write the discovery plan

Compile everything into one markdown document and save it where the user wants it (in a repo, follow its conventions for planning docs):

```
## Discovery Plan: [Topic]

**Date**: [today]
**Product stage**: [existing/new]
**Discovery question**: [what we're trying to learn]

### Ideas explored
[Brainstormed ideas with brief descriptions]

### Selected ideas for validation
[3-5 ideas carried forward, with rationale]

### Critical assumptions
| # | Assumption | Category | Impact | Uncertainty | Priority |
|---|-----------|----------|--------|-------------|----------|

### Validation experiments
| # | Tests assumption | Method | Success criteria | Effort | Timeline |
|---|-----------------|--------|-----------------|--------|----------|

### Experiment details
[For each experiment: hypothesis, setup, measurement, decision criteria]

### Timeline
Week 1: [experiments]
Week 2: [experiments]
Week 3: [analysis and decision]

### Decision framework
- If [experiment] succeeds → proceed to [next step]
- If [experiment] fails → [pivot / kill / investigate further]
```

### Step 7: Offer next steps

Suggest what fits: a PRD for the top idea, an interview script (**interview-script**) to go alongside the experiments, metrics to track them (**metrics-dashboard**), or a red-team of the plan (**strategy-red-team**).

## Notes

- At each checkpoint the user can redirect, skip a step, or go deeper.
- The discovery plan is a living document: offer to update it as experiments run.
- For new products, validate desirability before feasibility.
- For existing products, check whether usage data can answer an assumption before designing an experiment for it.
