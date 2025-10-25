---
name: product-design-toolkit
description: Comprehensive product design toolkit with dynamic skill routing across research, UI, interaction, testing, branding, and documentation disciplines
category: Design
tags: [product-design, ux, ui, research, design-systems, interaction-design, usability, documentation, branding, accessibility]
version: 1.0.0
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
Files: `/mnt/skills/user/product-designer/discovery/*.md`

### UI & Visual Design  
Load when: design systems, components, visual specs, handoffs
Files: `/mnt/skills/user/product-designer/ui-design/*.md`

### Interaction Design
Load when: animations, microinteractions, state flows
Files: `/mnt/skills/user/product-designer/interaction/*.md`

### Testing & Validation
Load when: usability tests, critiques, audits
Files: `/mnt/skills/user/product-designer/testing/*.md`

### Documentation
Load when: case studies, design decisions, presentations
Files: `/mnt/skills/user/product-designer/documentation/*.md`

## Decision Tree

**User mentions:** "interview", "research", "persona" 
→ Load discovery skills

**User mentions:** "component", "design system", "handoff", "accessibility"
→ Load ui-design skills

**User mentions:** "animation", "interaction", "microinteraction", "state"
→ Load interaction skills

**User mentions:** "usability test", "critique", "audit"
→ Load testing skills

**User mentions:** "case study", "portfolio", "document decision"
→ Load documentation skills

## Example Usage Pattern
```
User: "Help me plan user interviews for our checkout redesign"

Claude's process:
1. Recognize this is a discovery task
2. Use view tool: /mnt/skills/user/product-designer/discovery/user-interview-guide.md
3. Follow those specific instructions
4. Don't load other skills unless needed
```