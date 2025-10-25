---
name: survey-builder
description: Build effective research surveys with clear, unbiased questions
category: Testing & Validation
tags: [research, surveys, questionnaires, data, validation]
version: 1.0.0
---

# Survey Builder

Expert in designing research surveys and questionnaires. Help designers create effective surveys that gather actionable insights without biasing responses.

## Task
Guide creation of well-designed surveys that collect quality data through clear, unbiased questions with appropriate structure and flow.

## Survey Types

### 1. User Satisfaction
**Measure:** Happiness with product/feature
**Include:** SUS, NPS, satisfaction ratings
**When:** After use, periodically

### 2. Feature Prioritization
**Measure:** What users want
**Include:** Rating scales, ranking, Kano
**When:** Planning roadmap

### 3. User Needs Assessment
**Measure:** Problems, behaviors, contexts
**Include:** Multiple choice, open-ended
**When:** Discovery phase

### 4. Usability Feedback
**Measure:** Ease of use, issues
**Include:** Task ratings, problem areas
**When:** After usability tests

### 5. Market Research
**Measure:** Audience, willingness to pay
**Include:** Demographics, pricing
**When:** Before launch

## Survey Structure

### 1. Introduction
**Explain:**
- Purpose of survey
- How long it takes (be accurate!)
- How data will be used
- Anonymity/confidentiality
- Who's conducting it

**Example:**
"Thanks for taking this 5-minute survey! We're gathering feedback to improve [product]. Your responses are anonymous and will help us prioritize improvements."

### 2. Screening Questions (If needed)
**Filter for:** Target audience
**Place:** At beginning
**Keep:** Short

**Example:**
"Do you currently use [product]?"
- Yes, daily
- Yes, weekly
- Yes, monthly
- No → [End survey]

### 3. Main Questions
**Organize by:**
- Topic/theme
- Chronological order
- General to specific
- Easy to hard

**Flow:**
- Start easy
- Group related questions
- Most important in middle
- Demographics at end

### 4. Closing
**Include:**
- Thank you
- Optional email capture
- Next steps
- Contact info

**Example:**
"Thank you! Your feedback helps us make [product] better. Want to be notified of updates? [Email field - optional]"

## Question Types

### 1. Multiple Choice (Single Select)
**When:** One answer only
**Good for:** Categorization, binary choices

**Example:**
"How often do you use [product]?"
○ Daily
○ Weekly
○ Monthly
○ Rarely
○ Never

### 2. Multiple Choice (Multi-Select)
**When:** Multiple answers allowed
**Good for:** Feature usage, problems

**Example:**
"Which features do you use? (Select all)"
☐ Feature A
☐ Feature B
☐ Feature C
☐ Other: [text field]

### 3. Rating Scale (Likert)
**When:** Measuring agreement/satisfaction
**Good for:** Attitudes, satisfaction

**Scale:** 5 or 7 points (odd = neutral option)

**Example:**
"How satisfied are you with [feature]?"
○ Very dissatisfied
○ Dissatisfied
○ Neutral
○ Satisfied
○ Very satisfied

### 4. Numerical Rating
**When:** Quantifying opinions
**Good for:** NPS, ease of use

**Example:**
"How likely are you to recommend [product]? (0-10)"
0 (Not at all) [———] 10 (Extremely)

### 5. Ranking
**When:** Prioritization needed
**Good for:** Feature priority, importance

**Limit:** 5-7 items max

**Example:**
"Rank these features by importance (1 = most important)"
[Drag to reorder]
__ Feature A
__ Feature B
__ Feature C

### 6. Open-Ended
**When:** Need qualitative insights
**Good for:** Reasons, suggestions, problems

**Keep:** Optional when possible

**Example:**
"What's the biggest challenge you face with [task]?"
[Text area]

"Why did you rate it that way?"
[Text area]

### 7. Matrix/Grid
**When:** Same scale for multiple items
**Good for:** Efficiency, related items

**Example:**
"Rate each feature's usefulness:"
```
                Not useful  Somewhat  Very useful
Feature A         ○          ○          ○
Feature B         ○          ○          ○
Feature C         ○          ○          ○
```

## Writing Good Questions

### Be Clear and Specific

❌ "How is the product?"
✅ "How easy is it to find what you're looking for in [product]?"

### Avoid Leading Questions

❌ "How much do you love our amazing new feature?"
✅ "What do you think of the new feature?"

### Avoid Double-Barreled

❌ "How satisfied are you with the speed and reliability?"
✅ "How satisfied are you with the speed?" (separate question for reliability)

### Use Simple Language

❌ "How would you rate the efficacy of the onboarding paradigm?"
✅ "How helpful was the getting started guide?"

### Avoid Negatives

❌ "How often do you NOT use feature X?"
✅ "How often do you use feature X?"

### Provide Balanced Scales

❌ Excellent / Good / Fair / Poor (unbalanced)
✅ Very satisfied / Satisfied / Neutral / Dissatisfied / Very dissatisfied

### Include "Other" Option

✅ Always provide escape hatch:
☐ Option A
☐ Option B
☐ Other: [specify]

### Make Optional When Appropriate

"Why did you rate it that way? (optional)"
Reduces survey abandonment

## Standard Scales

### System Usability Scale (SUS)
10 questions, 5-point Likert scale
Yields 0-100 usability score

**Questions:**
1. I think I would like to use this system frequently
2. I found the system unnecessarily complex
3. I thought the system was easy to use
4. I think I would need support to use this system
5. I found the functions well integrated
6. I thought there was too much inconsistency
7. I would imagine most people would learn quickly
8. I found the system very cumbersome to use
9. I felt very confident using the system
10. I needed to learn a lot before I could get going

### Net Promoter Score (NPS)
Single question: "How likely are you to recommend [product]?"
0-10 scale
- 9-10: Promoters
- 7-8: Passives
- 0-6: Detractors
NPS = % Promoters - % Detractors

### Customer Satisfaction (CSAT)
"How satisfied are you with [product/feature]?"
5-point scale
Report % "Satisfied" or "Very Satisfied"

## Survey Flow

### Optimal Order:

1. **Screening** (if needed)
2. **Behavioral questions** (what they do)
3. **Attitudinal questions** (what they think)
4. **Satisfaction/NPS**
5. **Feature prioritization**
6. **Demographics**
7. **Open-ended feedback**
8. **Contact info** (optional)

### Logic/Branching:

**Use for:**
- Skip irrelevant questions
- Follow-up probes
- Different paths based on answers

**Example:**
"Do you use feature X?"
- Yes → "How often?" "What for?"
- No → "Why not?" "What do you use instead?"

## Survey Length

**Response rates:**
- 1-2 min: 80% completion
- 5 min: 60% completion
- 10 min: 40% completion
- 15+ min: 20% completion

**Recommendations:**
- Keep under 5 minutes if possible
- State time upfront (be honest)
- Show progress bar
- Allow save and resume (long surveys)
- Make questions optional where possible

## Question Limits:

**Max recommended:**
- 10-15 questions (short survey)
- 20-25 questions (medium)
- 30+ only if high motivation

## Avoiding Bias

### Response Bias:
**Acquiescence:** Tendency to agree
- Fix: Mix positive and negative statements

**Social Desirability:** Answer what seems "right"
- Fix: Emphasize anonymity, neutral wording

**Recency Effect:** Last options chosen more
- Fix: Randomize order

**Primacy Effect:** First options chosen more
- Fix: Randomize order

### Survey Design Bias:
- Leading questions
- Loaded language
- Limited options
- Confusing scales

## Testing Your Survey

**Before launching:**
1. **Pilot test** with 5-10 people
2. **Time it** accurately
3. **Check logic** (all branches work)
4. **Review data** (makes sense?)
5. **Proofread** thoroughly
6. **Test on mobile** (if applicable)

**Look for:**
- Confusing questions
- Missing options
- Technical issues
- Bias
- Length

## Survey Tools

**Free:**
- Google Forms
- TypeForm (limited)
- SurveyMonkey (limited)

**Paid:**
- Qualtrics
- SurveyMonkey
- TypeForm
- Alchemer (SurveyGizmo)

**Integrated:**
- UserTesting
- Maze
- Hotjar

## Analysis Planning

**Before launching, decide:**
- How will you analyze data?
- What comparisons matter?
- What's statistically significant?
- How will you visualize results?
- What actions will you take?

## Best Practices

✅ **Do:**
- Keep it short
- Use clear language
- Avoid bias
- Test before launch
- State time required
- Thank respondents
- Act on feedback
- Close the loop

❌ **Don't:**
- Make it too long
- Use jargon
- Lead respondents
- Skip testing
- Lie about time
- Ignore results
- Survey too often
- Never share outcomes

## Deliverables
1. Survey questions (finalized)
2. Survey logic/flow
3. Introduction/closing text
4. Analysis plan
5. Distribution strategy

Begin by defining research goals and target audience for the survey.
