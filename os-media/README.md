# Odd Scenes Agency - AI Operating System

An AI-powered operating system for running a boutique software design agency. This skill coordinates an entire team of specialized AI agents to handle client work, business operations, and lead generation.

## Overview

This is not a chatbot. It's a full agency team that can:
- Qualify leads and close deals
- Design and build software products
- Manage client relationships and support
- Handle accounting, legal, and security
- Run marketing campaigns and generate leads

The system is designed for a solo agency founder who wants to automate everything except high-level creative direction, complex technical decisions, and key client relationships.

## Architecture
```bash
/os-media/
├── SKILL.md # (Chief of Staff - coordinates everything)
├── README.md # (this file)
├── /product-team # (client deliverables)
│   ├── product-manager.md
│   ├── visual-designer.md
│   ├── product-designer.md
│   ├── frontend-dev.md
│   ├── backend-dev.md
│   ├── ai-dev.md
│   └── devops.md
├── /client-ops # (client-facing operations)
│   ├── support.md
│   └── legal.md
├── /internal-ops # (business operations)
│   ├── accounting.md
│   ├── strategy.md
│   └── security.md
└── /lead-gen # (growth & marketing)
    ├── sales.md
    ├── marketing-social.md
    ├── marketing-ads.md
    └── marketing-campaign.md
```

## How It Works

1. **You interact with the main skill** (SKILL.md acts as Chief of Staff)
2. **Work is routed to specialists** automatically based on the request
3. **Specialists collaborate** through the chief of staff coordination layer
4. **Critical decisions escalate** back to you when needed

## Usage Examples

### Client Project
```
You: "New inquiry from Acme Labs - want to build a DeFi dashboard"
System: 
  - Sales qualifies the lead
  - Product Manager scopes the project
  - Designers create mockups
  - Devs build it
  - DevOps deploys it
  - Support creates documentation
  → Surfaces key decisions/blockers to you along the way
```

### Marketing Campaign
```
You: "Launch campaign for our new AI design offering"
System:
  - Marketing Campaign creates strategy
  - Marketing Social drafts content
  - Marketing Ads sets up paid campaigns
  → Coordinates timing and messaging across channels
```

### Operations
```
You: "Invoice the Acme Labs project"
System:
  - Accounting generates invoice based on agreed terms
  - Sends it through appropriate channels
  - Tracks payment
```

## What Gets Automated

✅ Project scoping and requirements
✅ Design iterations (with your approval on major direction)
✅ Code implementation (with your review on complex logic)
✅ Infrastructure setup and deployment
✅ Client communication (standard updates, support)
✅ Lead outreach and qualification
✅ Content creation and ad campaigns
✅ Invoicing and financial tracking
✅ Contract review and legal basics

## What Needs You

⚠️ Creative direction on novel design problems
⚠️ Complex technical architecture decisions
⚠️ High-stakes client negotiations
⚠️ Business strategy and positioning
⚠️ Code review and testing before deployment
⚠️ Final approval on contracts and legal matters

## Integration Points

This skill connects to:
- **Gmail**: Client communication, lead outreach
- **Google Calendar**: Meetings, deadlines
- **Google Drive**: Documents, designs, deliverables
- **Notion**: Project tracking, documentation
- **Todoist**: Task management
- **Evernote**: Notes and research

## Getting Started

1. **Start with a real project**: "We have a new client who needs X"
2. **Let the system coordinate**: The chief of staff will route work and manage handoffs
3. **Review key decisions**: You'll be surfaced critical choices that need human judgment
4. **Iterate the team**: After a few projects, you'll see which roles need refinement

## Evolution Strategy

Built all roles upfront to test the full system, but expect to iterate:

**Phase 1** (first 2 weeks): Run real client work through the system, identify gaps
**Phase 2**: Refine the most-used roles (likely product-manager, frontend-dev, sales)
**Phase 3**: Add complexity to underutilized roles or merge redundant ones
**Phase 4**: Build custom integrations and automation workflows

## Philosophy

This isn't about replacing human creativity or judgment. It's about:
- Eliminating busywork and coordination overhead
- Scaling your personal capabilities
- Focusing your energy on the 20% of work that requires your unique skills
- Running a sustainable solo agency without burnout

The system is opinionated and proactive. Specialists don't wait for detailed instructions - they make smart decisions and escalate when needed.

## Notes

- Built for a designer/developer with 10+ years experience (assumes technical fluency)
- Optimized for small startup clients (web3, AI, SaaS, DeFi)
- Minimalist, fast-moving approach (not enterprise bureaucracy)
- Dark mode aesthetic preference, cyberpunk/futuristic lean
- Visual/diagram-heavy communication style

---

This is version 1.0. It will evolve as you use it.