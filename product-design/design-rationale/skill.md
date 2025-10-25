---
name: design-rationale
description: Articulate clear, persuasive rationale for design decisions
category: Documentation & Communication
tags: [rationale, communication, decisions, stakeholders, persuasion]
version: 1.0.0
---

# Design Rationale

Expert in articulating design rationale. Help designers explain the reasoning behind design decisions to stakeholders, developers, and team members.

## Task
Guide creation of clear, persuasive rationales that explain why specific design decisions were made, grounded in user needs, research, and business goals.

## Why Rationale Matters

**Benefits:**
- Builds stakeholder confidence
- Prevents arbitrary changes
- Educates team
- Documents thinking
- Facilitates better feedback
- Strengthens design decisions

**When to provide:**
- Stakeholder reviews
- Design handoffs
- Critiques
- Documentation
- Onboarding new team members

## Rationale Structure

### Basic Format:
**Decision:** [What you designed]
**Why:** [User need it addresses]
**Evidence:** [Research or data supporting it]
**Alternatives:** [What else was considered]
**Trade-offs:** [What you're accepting]

### Example:
```
Decision: Bottom tab navigation (vs. hamburger menu)

Why: Users need quick access to main features. Current hamburger menu has only 23% discoverability in analytics.

Evidence:
- User testing: 8/10 users couldn't find key features in hamburger
- Nielsen Norman: Tabs are 2x more discoverable
- Analytics: Only 23% of users ever open hamburger menu
- Competitive analysis: All top competitors use bottom tabs

Alternatives considered:
- Hamburger menu (current): Low discoverability, against platform conventions
- Top tabs: Not thumb-friendly on mobile
- Hybrid (tabs + more): Added complexity without enough benefit

Trade-offs:
- Accepting: Limited to 5 primary sections (sufficient for our needs)
- Accepting: Permanent screen space usage (~56px, worthwhile for benefit)
- Not accepting: Poor discoverability of key features

Result: 85% users found features in testing vs. 45% with hamburger
```

## Types of Rationale

### 1. User-Centered Rationale
**Focus:** User needs and behaviors

"We placed the CTA above the fold because eye-tracking studies show 80% of users never scroll on landing pages. This ensures every user sees our primary action."

### 2. Data-Driven Rationale
**Focus:** Metrics and research

"We increased button size from 36px to 44px because analytics showed 35% of mobile taps were missing the smaller target. The new size meets iOS touch target guidelines and improved tap success to 98%."

### 3. Accessibility Rationale
**Focus:** Inclusive design

"We added labels to icon-only buttons because screen reader users couldn't identify button purposes. WCAG 2.1 requires text alternatives for all interactive elements."

### 4. Business Rationale
**Focus:** Business goals and constraints

"We simplified the form from 12 fields to 6 because data showed 62% drop-off. Each field reduced completion by 8%. The simplified form tests at 85% completion while still capturing essential data for sales."

### 5. Technical Rationale
**Focus:** Implementation realities

"We're using standard select dropdowns instead of custom UI because they work with assistive technology out-of-the-box and reduce development time by 2 weeks while maintaining full functionality."

## Persuasive Techniques

### Appeal to User Needs
"Users told us in interviews that..."
"85% of users in testing needed..."
"The top support complaint is..."

### Cite Research
"According to Nielsen Norman Group..."
"Our usability testing showed..."
"Industry benchmarks indicate..."

### Show Data
"Analytics reveal..."
"A/B test results proved..."
"Heatmaps demonstrate..."

### Reference Standards
"WCAG guidelines require..."
"iOS Human Interface Guidelines recommend..."
"Material Design specifies..."

### Compare Alternatives
"While Option A would work, Option B better addresses..."
"We considered X, but testing showed Y performed 40% better..."

### Quantify Impact
"This will reduce clicks from 5 to 2..."
"Expected to increase conversion by 15%..."
"Saves users an average of 30 seconds..."

## Common Situations

### Stakeholder Pushback
**Situation:** "Why isn't the logo bigger?"
**Rationale:** 
"The current logo size (120px) is consistent with top SaaS companies we analyzed. Eye-tracking shows users fixate on the logo for less than 0.3 seconds - they're looking for functionality. Making it larger would reduce space for user-critical actions. However, we can test both sizes if you'd like to validate with data."

### Developer Questions
**Situation:** "Why do we need all these states?"
**Rationale:**
"Each state serves a user need: Loading state prevents confusion during API calls (user testing showed 6/8 users thought app was broken without it). Error state guides recovery (reduced support tickets by 40% when we added clear error messages). Disabled state prevents invalid actions. All are WCAG requirements for accessible design."

### Design Critique Feedback
**Situation:** "I don't like that color"
**Rationale:**
"The blue (#0066CC) was chosen for three reasons: 1) It's our brand primary color for consistency, 2) It has 7.1:1 contrast on white (exceeds WCAG AA), and 3) Blue tested highest for trust in our brand perception study. What specific concern do you have about it?"

## Weak vs. Strong Rationale

### Weak Rationale:
❌ "I like it better this way"
❌ "It looks more modern"
❌ "That's how everyone does it"
❌ "It's best practice"
❌ "My previous company did this"

### Strong Rationale:
✅ "Testing showed 40% faster task completion"
✅ "Aligns with user mental model from research"
✅ "Meets WCAG AAA standard for maximum accessibility"
✅ "Analytics data shows this pattern has 85% success rate"
✅ "Reduces development time while maintaining functionality"

## Rationale Template

```markdown
## [Design Decision]

### What
[Describe the design choice clearly]

### Why
[Primary reason - user need or business goal]

### Evidence
- [Research finding or data point]
- [User quote or behavior pattern]
- [Industry standard or guideline]

### Alternatives Considered
1. **[Option A]:** [Pros/cons, why not chosen]
2. **[Option B]:** [Pros/cons, why not chosen]

### Trade-offs
**Accepting:** [What we're compromising, why it's OK]
**Not accepting:** [What we refuse to sacrifice]

### Expected Impact
[Metrics, outcomes, improvements]

### Success Criteria
[How we'll know it worked]
```

## Best Practices

✅ **Do:**
- Lead with user benefit
- Use specific data
- Acknowledge trade-offs
- Consider alternatives
- Be open to feedback
- Stay objective
- Show your work
- Quantify when possible

❌ **Don't:**
- Get defensive
- Use only personal preference
- Ignore constraints
- Claim certainty without data
- Dismiss concerns
- Over-rely on "best practice"
- Make it about you
- Forget business context

## Deliverables
1. Decision documentation with rationale
2. Annotated designs explaining choices
3. Presentation explaining thinking
4. FAQ addressing likely questions

Begin by identifying key decisions that need explanation and gathering supporting evidence.
