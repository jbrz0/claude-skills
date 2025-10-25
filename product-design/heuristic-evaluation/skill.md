---
name: heuristic-evaluation
description: Conduct systematic heuristic evaluations using Nielsen's principles
category: Critique & Evaluation
tags: [heuristics, usability, evaluation, nielsen, ux-audit]
version: 1.0.0
---

# Heuristic Evaluation

Expert in conducting heuristic evaluations using Nielsen's usability heuristics and other evaluation frameworks. Help designers systematically evaluate interfaces for usability issues.

## Task
Guide systematic evaluation of user interfaces against established usability principles to identify problems before user testing.

## Nielsen's 10 Usability Heuristics

### 1. Visibility of System Status
**Principle:** Keep users informed about what's going on
**Check for:**
- Loading indicators
- Progress bars
- Current location (breadcrumbs)
- System feedback (confirmations, errors)
- Real-time updates

**Common violations:**
- No feedback after actions
- Unclear current state
- Missing progress indicators

### 2. Match Between System and Real World
**Principle:** Speak the user's language
**Check for:**
- Familiar terms and concepts
- Real-world metaphors
- Logical information flow
- User's mental model

**Common violations:**
- Technical jargon
- Confusing metaphors
- Illogical organization

### 3. User Control and Freedom
**Principle:** Users need emergency exits
**Check for:**
- Undo/redo
- Cancel operations
- Exit flows easily
- Back button works

**Common violations:**
- No way to undo
- Can't cancel processes
- Trapped in wizards

### 4. Consistency and Standards
**Principle:** Follow platform and industry conventions
**Check for:**
- Consistent terminology
- Standard UI patterns
- Predictable behavior
- Platform conventions

**Common violations:**
- Inconsistent labels
- Reinventing common patterns
- Breaking platform norms

### 5. Error Prevention
**Principle:** Prevent problems before they occur
**Check for:**
- Confirmations for destructive actions
- Input constraints
- Clear defaults
- Helpful formatting
- Inline validation

**Common violations:**
- No confirmation for delete
- Accepting invalid input
- Easy to make mistakes

### 6. Recognition Rather Than Recall
**Principle:** Minimize memory load
**Check for:**
- Visible options
- Clear instructions
- Contextual help
- Autocomplete
- Recently used items

**Common violations:**
- Hidden functionality
- Complex commands to remember
- No help available

### 7. Flexibility and Efficiency
**Principle:** Accelerators for expert users
**Check for:**
- Keyboard shortcuts
- Customization options
- Bulk actions
- Templates
- Saved preferences

**Common violations:**
- No shortcuts
- Can't customize
- Must repeat tasks

### 8. Aesthetic and Minimalist Design
**Principle:** Dialogue should not contain irrelevant information
**Check for:**
- Clear visual hierarchy
- Only necessary information
- Uncluttered interface
- Focused content

**Common violations:**
- Information overload
- Unnecessary decoration
- Competing elements

### 9. Help Users Recognize, Diagnose, and Recover from Errors
**Principle:** Error messages should be helpful
**Check for:**
- Plain language errors
- What went wrong
- How to fix it
- Constructive tone

**Common violations:**
- Error codes only
- Vague messages
- No solution provided

### 10. Help and Documentation
**Principle:** Provide help when needed
**Check for:**
- Easy to search
- Focused on tasks
- Concrete steps
- Contextual help
- Not too large

**Common violations:**
- No documentation
- Hard to find help
- Overwhelming docs

## Evaluation Process

### 1. Preparation
- Understand the product
- Define scope (entire app or specific flows)
- Gather evaluators (3-5 ideal)
- Create evaluation form

### 2. Individual Evaluation
Each evaluator independently:
- Goes through interface
- Checks against each heuristic
- Notes violations
- Rates severity
- Takes screenshots

### 3. Severity Rating

**0 - Not a problem**
Doesn't violate heuristic

**1 - Cosmetic**
Doesn't need to be fixed unless extra time

**2 - Minor**
Low priority fix

**3 - Major**
Important to fix, high priority

**4 - Catastrophic**
Must fix before release

**Consider:**
- Frequency (how often occurs)
- Impact (how bad when it occurs)
- Persistence (one-time or repeated)

### 4. Consolidation
- Combine all evaluators' findings
- Remove duplicates
- Discuss disagreements
- Average severity ratings
- Prioritize issues

### 5. Reporting
- List all issues
- Group by heuristic
- Include screenshots
- Provide recommendations
- Prioritize fixes

## Evaluation Template

```markdown
## Issue #[N]

**Heuristic Violated:** [Which of 10]

**Location:** [Where in interface]

**Description:** [What's wrong]

**Severity:** [0-4]
- Frequency: [How often]
- Impact: [How severe]  
- Persistence: [One-time or ongoing]

**Recommendation:** [How to fix]

**Screenshot:** [Image]
```

## Example Issues

**Issue #1**
Heuristic: Error Prevention (#5)
Location: Checkout - Delete cart item
Description: No confirmation when deleting items from cart. Users can accidentally remove items with no way to undo.
Severity: 3 (Major)
- Frequency: Common (many items managed)
- Impact: High (lose shopping progress)
- Persistence: Repeated use
Recommendation: Add confirmation dialog "Remove [item] from cart?" with Cancel and Remove buttons.

**Issue #2**
Heuristic: Visibility of System Status (#1)
Location: File upload
Description: No progress indicator during upload. Users don't know if upload is working or how long it will take.
Severity: 3 (Major)
- Frequency: Every upload
- Impact: High (uncertainty, may abandon)
- Persistence: Every time
Recommendation: Add progress bar showing upload percentage and estimated time remaining.

## Variations & Extensions

### Mobile Heuristics
Additional considerations:
- Touch target size (44×44px min)
- Thumb-friendly zones
- One-handed use
- Orientation changes
- Network variability

### Accessibility Heuristics
Check for:
- Keyboard navigation
- Screen reader support
- Color contrast
- Focus indicators
- Alt text

### Domain-Specific
- E-commerce (trust signals, checkout flow)
- Enterprise (data density, efficiency)
- Social (privacy, moderation)

## Best Practices

**Do:**
✅ Have multiple evaluators
✅ Be systematic (check every screen)
✅ Focus on user needs
✅ Provide specific examples
✅ Suggest solutions
✅ Prioritize issues
✅ Follow up with user testing

**Don't:**
❌ Rely on one evaluator
❌ Skip screens
❌ Just list problems
❌ Be vague
❌ Only criticize
❌ Ignore severity
❌ Replace user testing

## Advantages
- Quick and cheap
- No users needed
- Finds many issues
- Early in process
- Expert perspective

## Limitations
- Misses some user issues
- Evaluator bias
- No user behavior data
- May find false positives
- Doesn't validate solutions

## Deliverables
1. Heuristic evaluation report
2. Issue list (prioritized)
3. Screenshots/annotations
4. Recommendations
5. Summary presentation

Begin by defining scope and assembling evaluators for systematic review.
