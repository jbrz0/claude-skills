---
name: ab-test-hypothesis
description: Formulate clear, testable hypotheses for A/B tests and experiments
category: Testing & Validation
tags: [testing, ab-testing, experimentation, hypothesis, metrics]
version: 1.0.0
---

# A/B Test Hypothesis

Expert in formulating A/B test hypotheses. Help designers create clear, testable hypotheses that drive meaningful experiments and learning.

## Task
Guide creation of well-structured A/B test hypotheses that are specific, measurable, and tied to user insights or business goals.

## A/B Test Hypothesis Format

### Standard Format:
**If** [we make this change]
**Then** [this metric will change]
**Because** [this is our reasoning]

### Example:
"If we change the CTA button from 'Submit' to 'Get Started',
Then we'll see a 10% increase in click-through rate,
Because 'Get Started' is more action-oriented and less intimidating than 'Submit' based on user interviews."

## Hypothesis Components

### 1. Independent Variable (What Changes)
**The change you're testing:**
- Specific and clear
- One variable at a time
- Implementable

**Good:**
- "Change button color from gray to blue"
- "Add security badge next to payment form"
- "Reduce form fields from 8 to 4"

**Bad:**
- "Make it better"
- "Change everything"
- "Test multiple buttons and forms"

### 2. Dependent Variable (What Measures)
**The metric you're tracking:**
- Measurable
- Relevant to business goals
- Detectable change

**Common metrics:**
- Conversion rate
- Click-through rate
- Time on task
- Bounce rate
- Revenue per visitor
- Sign-up rate
- Completion rate

### 3. Rationale (Why)
**Your reasoning:**
- Based on research or data
- User behavior insight
- Psychological principle
- Industry knowledge

**Evidence types:**
- User research findings
- Analytics data
- Heuristic principles
- Competitor analysis
- Psychological theory

## Types of A/B Tests

### 1. Visual Design
**Test:** Color, size, layout, typography

**Example Hypothesis:**
"If we increase the CTA button size from 36px to 48px, then mobile conversion will increase by 15%, because current analytics show 30% tap errors on the smaller button."

### 2. Copy/Content
**Test:** Headlines, button labels, descriptions

**Example:**
"If we change headline from 'Enterprise Software' to 'Grow Your Business Faster', then sign-ups will increase by 20%, because user interviews showed users don't relate to 'enterprise' but do want growth."

### 3. Layout/Structure
**Test:** Element placement, page structure

**Example:**
"If we move testimonials above pricing table, then plan selection will increase by 10%, because trust signals (testimonials) should precede commitment decisions."

### 4. Interaction
**Test:** Buttons vs. links, modals vs. inline

**Example:**
"If we change from modal popup to inline form, then form completion will increase by 25%, because users in testing felt trapped by modals and abandoned."

### 5. Urgency/Scarcity
**Test:** Limited time, stock indicators

**Example:**
"If we add 'Only 3 spots left' indicator, then registration will increase by 15%, because scarcity principles create urgency (Cialdini)."

## Hypothesis Quality Criteria

### Good Hypothesis Is:

**Specific:**
❌ "If we improve the homepage, conversions will increase"
✅ "If we add customer logos above the fold, sign-ups will increase by 12%"

**Measurable:**
❌ "Users will like it better"
✅ "Click-through rate will increase from 3% to 4%"

**Testable:**
❌ "If we make it more modern"
✅ "If we change from serif to sans-serif font"

**Has Clear Rationale:**
❌ "Because it looks better"
✅ "Because readability studies show sans-serif performs 15% better on screens"

**Realistic:**
❌ "Conversion will increase 500%"
✅ "Conversion will increase 10-15%"

## Hypothesis Development Process

### 1. Identify Opportunity
**Sources:**
- Analytics (drop-off points)
- User research (pain points)
- Heuristic review (violations)
- Customer feedback (complaints)
- Competitive analysis (gaps)

### 2. Understand Root Cause
**Ask why:**
- Why are users dropping off here?
- Why isn't this working?
- What's the user need?
- What's the barrier?

### 3. Generate Solution Ideas
**Brainstorm changes:**
- What could fix this?
- What have others done?
- What does research suggest?

### 4. Prioritize Tests
**Consider:**
- Potential impact (high/medium/low)
- Ease of implementation (easy/hard)
- Learning value (insight gained)
- Risk level (safe to test?)

**ICE Score:**
Impact × Confidence × Ease

### 5. Write Hypothesis
Follow format with evidence

### 6. Define Success Metrics
**Primary:** Main metric
**Secondary:** Supporting metrics
**Guardrail:** Metrics that shouldn't worsen

## Example Hypotheses

### Good Examples:

**E-commerce Checkout:**
"If we add progress indicator to multi-step checkout, then completion rate will increase from 65% to 72%, because user testing showed 8/10 users felt lost and unsure how many steps remained."

**SaaS Sign-up:**
"If we remove phone number field from sign-up form, then sign-up conversion will increase by 18%, because analytics show 40% of drop-offs occur at this field and user interviews revealed privacy concerns."

**Landing Page:**
"If we replace stock photo with product screenshot, then demo requests will increase by 15%, because eye-tracking studies show users skip generic imagery but engage with UI screenshots."

**Pricing Page:**
"If we highlight the middle-tier plan with 'Most Popular' badge, then middle-tier selections will increase from 30% to 45%, because choice architecture research shows defaults and social proof drive decisions."

**Email Campaign:**
"If we change subject line from 'Newsletter #47' to 'Your Weekly Design Tips', then open rate will increase from 18% to 25%, because our previous tests show personalized, benefit-focused subject lines outperform generic ones by 35%."

### Common Mistakes:

**Too vague:**
❌ "If we improve the homepage, metrics will get better"

**No rationale:**
❌ "If we make button blue, clicks will increase by 20%"

**Multiple variables:**
❌ "If we change color, size, and copy, then clicks will increase"

**Unrealistic:**
❌ "If we add one word, revenue will increase 400%"

**Not measurable:**
❌ "If we redesign, users will be happier"

## Test Planning

### Sample Size Calculator
**Need to determine:**
- Baseline conversion rate
- Minimum detectable effect
- Statistical significance (95% typical)
- Statistical power (80% typical)

### Test Duration
**Consider:**
- Weekly cycles (full weeks)
- Seasonal effects
- Traffic volume
- Minimum 1-2 weeks

### Success Criteria
**Define before testing:**
- What change = success?
- Statistical significance level
- Practical significance (is change meaningful?)

## Documentation Template

```markdown
## A/B Test: [Test Name]

### Hypothesis
If [change],
Then [metric impact],
Because [rationale].

### Current State
- Metric: [Current value]
- Sample: [Where/who]
- Timeframe: [Data source period]

### Proposed Change
**Variant A (Control):** [Current design]
**Variant B:** [Proposed change]

[Screenshots or descriptions]

### Rationale
**Evidence:**
- [User research finding]
- [Analytics data]
- [Industry standard]

**Why this will work:**
[Explanation of mechanism]

### Success Metrics
**Primary:** [Main metric to move]
- Current: [X%]
- Target: [Y%] (Z% increase)

**Secondary:**
- [Supporting metric 1]
- [Supporting metric 2]

**Guardrails:**
- [Metric that shouldn't worsen]

### Test Parameters
- Traffic split: 50/50
- Minimum sample: [N per variant]
- Duration: [Days/weeks]
- Statistical significance: 95%

### Risks
- [Potential downside]
- [Mitigation plan]

### Next Steps
If successful: [Implementation plan]
If unsuccessful: [Learning and next test]
```

## Best Practices

✅ **Do:**
- Base on research/data
- Test one variable at a time
- Define success beforehand
- Run to statistical significance
- Document everything
- Learn from failures
- Iterate and retest

❌ **Don't:**
- Guess without evidence
- Test multiple changes together
- Stop tests early
- Ignore guardrail metrics
- Test without rationale
- Only test wins
- Forget to implement winners

## Deliverables
1. Test hypothesis document
2. Variant specifications
3. Success criteria
4. Test plan
5. Results analysis framework

Begin by identifying conversion bottlenecks or user pain points to test against.
