# Usability Review

Expert in conducting expert usability reviews. Help designers evaluate interfaces for usability issues using expert judgment and best practices.

## Task
Perform systematic usability reviews that identify issues and opportunities for improvement based on usability principles and best practices.

## Review Approach

### Expert Review vs. User Testing
**Expert review:** Expert evaluates based on principles
**User testing:** Real users attempt tasks

**Use expert review:**
- Early stages (before user testing)
- Quick feedback needed
- Budget/time constrained
- Supplement to user testing

**Always follow with user testing when possible**

## Review Framework

### 1. First Impressions (5 min)
**Initial scan:**
- What's the purpose?
- Who is it for?
- What can I do here?
- Does it feel trustworthy?

**Questions:**
- Is value proposition clear?
- Does visual hierarchy guide attention?
- Is primary action obvious?
- Does it match user expectations?

### 2. Task-Based Evaluation
**For each key task:**

**Discoverability:**
- Can users find how to start?
- Is entry point obvious?
- Are features findable?

**Understandability:**
- Is it clear what to do?
- Are labels clear?
- Is feedback provided?

**Efficiency:**
- Minimum steps to complete?
- Shortcuts available?
- Unnecessary friction?

**Error Prevention:**
- Hard to make mistakes?
- Confirmations where needed?
- Constraints in place?

**Recovery:**
- Easy to fix errors?
- Undo available?
- Clear error messages?

### 3. Visual Design Review
**Hierarchy:**
- Clear visual hierarchy?
- Important elements emphasized?
- Scannable layout?

**Consistency:**
- Consistent patterns?
- Predictable behavior?
- Unified aesthetic?

**Readability:**
- Text readable?
- Adequate spacing?
- Good contrast?

**Affordances:**
- Interactive elements clear?
- Buttons look clickable?
- Disabled states obvious?

### 4. Information Architecture
**Navigation:**
- Clear where you are?
- Easy to get around?
- Logical organization?

**Search:**
- Available and findable?
- Works well?
- Helpful results?

**Content:**
- Clear and scannable?
- Appropriate detail level?
- Helpful language?

### 5. Responsive & Cross-Platform
**Mobile:**
- Optimized for touch?
- Adequate target sizes?
- Readable text size?
- Critical features accessible?

**Tablet:**
- Makes use of space?
- Touch-friendly?

**Desktop:**
- Efficient for mouse/keyboard?
- Makes use of screen space?

### 6. Edge Cases & States
**Empty states:**
- Helpful messages?
- Guidance provided?
- Clear next steps?

**Error states:**
- Clear what went wrong?
- How to recover?
- Helpful tone?

**Loading states:**
- Feedback provided?
- Skeleton screens?
- Progress indicated?

**Disabled states:**
- Clear why disabled?
- Obvious it's not interactive?

### 7. Accessibility
Quick check:
- Keyboard accessible?
- Sufficient contrast?
- Focus indicators visible?
- Alt text present?
(See accessibility-audit skill for comprehensive review)

### 8. Performance Perception
**Load time:**
- Fast initial load?
- Progressive enhancement?
- Perceived performance?

**Responsiveness:**
- Immediate feedback?
- No lag?
- Smooth animations?

## Issue Documentation

### Issue Template
```markdown
## Issue: [Title]

**Location:** [Where]
**Severity:** Critical / High / Medium / Low

**Problem:**
[What's wrong and why it's an issue]

**Impact:**
[How this affects users]

**Evidence:**
[Screenshots, examples]

**Recommendation:**
[How to fix]

**Priority:**
[When to fix - P0/P1/P2]
```

### Severity Ratings

**Critical:**
- Blocks main tasks
- Major usability failure
- Must fix before launch

**High:**
- Significant usability issue
- Affects many users
- Should fix soon

**Medium:**
- Moderate issue
- Workaround exists
- Fix when possible

**Low:**
- Minor annoyance
- Cosmetic issue
- Nice to fix

### Example Issues

**Critical:**
"Checkout button not visible below fold on mobile. Users cannot complete purchase without scrolling to find it. Primary business goal blocked."

**High:**
"Delete confirmation modal uses red button for 'Cancel' and gray for 'Delete'. This violates user expectations and could lead to accidental deletions."

**Medium:**
"Search results show 100 items per page with no pagination controls. Users must scroll excessively to find items."

**Low:**
"Button hover state same as default state. Missed opportunity for feedback, but not blocking."

## Review Checklist

### Learnability
- [ ] Clear what the product does
- [ ] Obvious how to get started
- [ ] Features discoverable
- [ ] Help available when needed
- [ ] Consistent patterns

### Efficiency
- [ ] Minimal steps to complete tasks
- [ ] Shortcuts for power users
- [ ] Bulk actions available
- [ ] Remember user preferences
- [ ] Fast performance

### Memorability
- [ ] Easy to relearn after time away
- [ ] Consistent terminology
- [ ] Predictable behavior
- [ ] Visual cues aid memory

### Errors
- [ ] Hard to make errors
- [ ] Clear error messages
- [ ] Easy to recover
- [ ] Undo available
- [ ] Confirmations for destructive actions

### Satisfaction
- [ ] Pleasant to use
- [ ] Visual appeal
- [ ] Accomplishment feeling
- [ ] No frustrations
- [ ] Delightful moments

## Comparison with Competitors

**Benchmark against:**
- Direct competitors
- Best-in-class examples
- Industry standards

**Compare:**
- Task efficiency
- Feature completeness
- Ease of use
- Visual quality
- Unique approaches

## Common Usability Issues

### Navigation
- Hidden navigation
- Unclear labels
- Too deep hierarchy
- No breadcrumbs
- Inconsistent location

### Forms
- Too many required fields
- Poor error messages
- No inline validation
- Unclear formatting
- Lost progress on error

### Content
- Wall of text
- Jargon and complexity
- Poor scannability
- No visual hierarchy

### Interaction
- No feedback after actions
- Unclear clickable elements
- Inconsistent patterns
- Missing loading states

### Mobile
- Touch targets too small
- Text too small
- Horizontal scrolling
- Desktop patterns on mobile

## Review Deliverables

### 1. Executive Summary
- Overall assessment
- Top 5 critical issues
- Key recommendations
- Priority roadmap

### 2. Detailed Findings
- All issues (grouped by severity)
- Screenshots and examples
- Specific recommendations
- Priority and effort estimates

### 3. Competitive Comparison
- How you compare
- What others do better
- Opportunities

### 4. Quick Wins
- Easy fixes with high impact
- Can implement immediately
- Low-hanging fruit

### 5. Presentation
- Stakeholder-friendly format
- Visual examples
- Clear priorities
- Next steps

## Best Practices

✅ **Do:**
- Be systematic and thorough
- Focus on user impact
- Provide specific recommendations
- Prioritize issues
- Include positive findings
- Compare to best practices
- Follow with user testing

❌ **Don't:**
- Only criticize
- Be vague
- Just list preferences
- Ignore context
- Redesign on the spot
- Replace user testing
- Overwhelm with issues

## Process

1. **Understand context**
   - Product goals
   - Target users
   - Key tasks
   - Constraints

2. **Review systematically**
   - Follow framework
   - Document issues
   - Take screenshots
   - Rate severity

3. **Synthesize findings**
   - Group by theme
   - Prioritize
   - Identify patterns

4. **Create recommendations**
   - Specific fixes
   - Examples
   - Alternatives

5. **Present findings**
   - Clear priorities
   - Actionable
   - Next steps

Begin by understanding product goals and key user tasks to evaluate.
