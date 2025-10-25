---
name: "product-design-toolkit"
description: "Comprehensive product design toolkit with dynamic skill routing across research, UI, interaction, testing, branding, and documentation disciplines"
category: "Design"
tags: ["product-design", "ux", "ui", "research", "design-systems", "interaction-design", "usability", "documentation", "branding", "accessibility"]
version: "1.0.0"
---

# Product Designer Toolkit

## Description
Comprehensive product design skills covering research, UI, interaction, documentation, and validation. Dynamically loads relevant sub-skills based on task type.

## How to Use This Skill

1. **Analyze the user's request** to determine which design discipline(s) are needed
2. **Load only the relevant sub-skill files** using the `view` tool
3. **Follow the instructions** in those specific sub-skills
4. **Don't load all sub-skills** - only what's needed for the current task

## Skill Categories & When to Load

### Discovery & Research
Load when: user research, interviews, personas, journey maps, problem framing
Files: `/mnt/skills/user/product-design-toolkit/discovery/*.md`

### Strategy & Planning
Load when: IA, design sprints, prioritization, user stories, stakeholder work
Files: `/mnt/skills/user/product-design-toolkit/strategy/*.md`

### UI & Visual Design  
Load when: design systems, components, visual specs, handoffs, color, typography
Files: `/mnt/skills/user/product-design-toolkit/ui-design/*.md`

### Interaction Design
Load when: animations, microinteractions, state flows, error states
Files: `/mnt/skills/user/product-design-toolkit/interaction/*.md`

### Branding & Art Direction
Load when: brand strategy, visual identity, mood boards, brand voice
Files: `/mnt/skills/user/product-design-toolkit/branding/*.md`

### Critique & Evaluation
Load when: design critiques, heuristic evaluations, accessibility audits, usability reviews
Files: `/mnt/skills/user/product-design-toolkit/critique/*.md`

### Documentation
Load when: case studies, design decisions, presentations, portfolio, rationale
Files: `/mnt/skills/user/product-design-toolkit/documentation/*.md`

### Testing & Validation
Load when: usability tests, A/B tests, test scripts, surveys
Files: `/mnt/skills/user/product-design-toolkit/testing/*.md`

### Workflow & Process
Load when: design briefs, kickoffs, estimation, feedback synthesis, QA checklists
Files: `/mnt/skills/user/product-design-toolkit/workflow/*.md`

## Decision Tree

**User mentions:** "interview", "research", "persona", "journey", "empathy map"
→ Load discovery skills

**User mentions:** "information architecture", "IA", "sitemap", "sprint", "prioritize", "user story"
→ Load strategy skills

**User mentions:** "component", "design system", "handoff", "accessibility", "color", "typography", "icon"
→ Load ui-design skills

**User mentions:** "animation", "interaction", "microinteraction", "state", "error"
→ Load interaction skills

**User mentions:** "brand", "visual identity", "mood board", "brand voice", "art direction"
→ Load branding skills

**User mentions:** "critique", "heuristic", "audit", "usability review"
→ Load critique skills

**User mentions:** "case study", "portfolio", "document decision", "presentation", "rationale"
→ Load documentation skills

**User mentions:** "usability test", "A/B test", "test script", "survey"
→ Load testing skills

**User mentions:** "design brief", "kickoff", "estimate", "feedback", "QA checklist"
→ Load workflow skills

## Example Usage Pattern
```
User: "Help me plan user interviews for our checkout redesign"

Claude's process:
1. Recognize this is a discovery task
2. Use view tool: /mnt/skills/user/product-design-toolkit/discovery/user-interview-guide.md
3. Follow those specific instructions
4. Don't load other skills unless needed
```
