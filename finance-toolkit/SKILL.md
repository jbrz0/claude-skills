---
name: finance-toolkit
description: Personal finance management across budgeting, investing, options trading, and financial planning
---

# Finance Toolkit

## Description
Comprehensive personal finance skills covering budgeting, investment management, options trading strategies, financial planning, and tax optimization. Dynamically loads relevant sub-skills based on task type.

## How to Use This Skill

1. **Analyze the user's request** to determine which finance domain is needed
2. **Load only the relevant sub-skill files** using the `view` tool
3. **Follow the instructions** in those specific sub-skills
4. **Don't load all sub-skills** - only what's needed for the current task

## Skill Categories & When to Load

### Budget Management
Load when: budget review, spending analysis, category tracking, expense optimization
Files: `/mnt/skills/user/finance-toolkit/budget/*.md`

### Investments
Load when: portfolio review, stock analysis, crypto tracking, rebalancing, performance analysis, research reports
Files: `/mnt/skills/user/finance-toolkit/investments/*.md`

### Options Trading
Load when: wheel strategy, butterflies, condors, spreads, options analysis, position management, strike selection
Files: `/mnt/skills/user/finance-toolkit/trading/*.md`

### Financial Planning
Load when: insurance review, retirement planning, subscriptions audit, long-term goals, financial strategy
Files: `/mnt/skills/user/finance-toolkit/planning/*.md`

### Tax Optimization
Load when: tax-loss harvesting, deductions, quarterly estimates, tax strategy, year-end planning
Files: `/mnt/skills/user/finance-toolkit/tax/*.md`

## Decision Tree

**User mentions:** "budget", "spending", "expenses", "categories", "monthly review", "burn rate"
→ Load budget/budget-manager.md

**User mentions:** "portfolio", "allocation", "rebalancing", "performance", "holdings", "asset mix"
→ Load investments/portfolio-manager.md

**User mentions:** "research", "DD", "analysis" + stock ticker
→ Load investments/equity-research.md

**User mentions:** "crypto", "defi", "token", "protocol", "on-chain" + project/coin name
→ Load investments/crypto-research.md

**User mentions:** "wheel", "covered call", "cash-secured put", "CSP", "CC", "selling premium", "theta"
→ Load trading/options-wheel.md

**User mentions:** "butterfly", "condor", "iron", "spread", "broken wing", "defined risk"
→ Load trading/options-advanced.md

**User mentions:** "call", "put", "directional", "long", "buying options", "OTM", "lottery"
→ Load trading/directional-plays.md

**User mentions:** "insurance", "coverage", "policy", "life insurance", "disability", "umbrella"
→ Load planning/insurance-advisor.md

**User mentions:** "retirement", "401k", "IRA", "Roth", "pension", "FIRE", "savings rate"
→ Load planning/retirement-planner.md

**User mentions:** "subscriptions", "recurring", "monthly costs", "cancel", "SaaS spending"
→ Load planning/subscription-audit.md

**User mentions:** "tax", "deduction", "harvesting", "write-off", "quarterly", "1099", "tax loss"
→ Load tax/tax-optimizer.md

## Integration Points

**Data Sources (via MCPs when available):**
- Budget sheet: Google Sheets
- Investment tracking: Google Sheets / Notion
- Tax documents: Google Drive
- Subscriptions: Notion / Evernote
- Notes: Evernote

**Without MCPs:**
- User provides data manually
- Work from uploaded files
- Build tracking templates

## Cross-Module Workflows

Some tasks require multiple modules:

**Portfolio rebalancing + tax optimization:**
→ Load investments/portfolio-manager.md AND tax/tax-optimizer.md

**Options income + budget planning:**
→ Load trading/options-wheel.md AND budget/budget-manager.md

**Retirement contribution + tax strategy:**
→ Load planning/retirement-planner.md AND tax/tax-optimizer.md

**Stock research before selling puts:**
→ Load investments/equity-research.md AND trading/options-wheel.md

**Complete financial review:**
→ Load budget/budget-manager.md, investments/portfolio-manager.md, planning/retirement-planner.md

## Example Usage Pattern
```
User: "I want to research NVDA before selling a put on it"

Claude's process:
1. Recognize: stock research + options trading
2. Load: investments/equity-research.md
3. Load: trading/options-wheel.md
4. First: Generate research report on NVDA
5. Then: Analyze if good wheel candidate
6. Output: Research + strike/expiration recommendation
```

## Global Financial Context

**Risk Profile:** [To be defined in each sub-skill]
**Time Horizon:** [To be defined]
**Goals:** [To be defined]
**Constraints:** [To be defined]

Each sub-skill will ask for specific context on first use.