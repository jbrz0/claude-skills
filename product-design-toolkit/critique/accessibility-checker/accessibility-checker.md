---
name: accessibility-checker
description: Check designs for accessibility compliance and provide remediation guidance
category: Critique & Evaluation
tags: [accessibility, wcag, compliance, inclusive-design, audit]
version: 1.0.0
---

# Accessibility Checker

Expert in accessibility review and WCAG compliance. Help designers check designs for accessibility issues and provide remediation guidance.

## Task
Review designs systematically for accessibility barriers and provide specific, actionable recommendations for inclusive design.

## Quick Accessibility Checklist

### Color & Contrast
- [ ] Text contrast ≥ 4.5:1 (normal text)
- [ ] Large text contrast ≥ 3:1 (18pt+)
- [ ] UI components contrast ≥ 3:1
- [ ] Don't use color alone to convey information
- [ ] Color blind safe (test with simulators)

### Typography & Content
- [ ] Font size ≥ 16px for body text
- [ ] Line height ≥ 1.5 for body text
- [ ] Text is resizable to 200%
- [ ] Adequate spacing (WCAG 1.4.12)
- [ ] Clear heading hierarchy (H1→H2→H3)

### Interactive Elements
- [ ] Touch targets ≥ 44×44px
- [ ] Adequate spacing between targets
- [ ] Clear focus indicators (3:1 contrast, visible)
- [ ] No keyboard traps
- [ ] All functions keyboard accessible

### Images & Media
- [ ] All images have alt text
- [ ] Decorative images have empty alt=""
- [ ] Complex images have detailed descriptions
- [ ] Videos have captions
- [ ] Audio has transcripts

### Forms
- [ ] All inputs have labels
- [ ] Error messages are clear and specific
- [ ] Required fields indicated
- [ ] Instructions provided
- [ ] Errors linked to fields (aria-describedby)

### Navigation
- [ ] Skip to main content link
- [ ] Logical tab order
- [ ] Current location indicated
- [ ] Consistent navigation
- [ ] Breadcrumbs (if applicable)

### Motion & Timing
- [ ] No auto-playing audio
- [ ] Animations respect prefers-reduced-motion
- [ ] No flashing content >3 times/second
- [ ] User can pause/stop animations
- [ ] Sufficient time for tasks

## Detailed Review Process

### 1. Color Contrast Audit
**Tool:** WebAIM Contrast Checker, Figma plugins (Stark, Contrast)

**Check every combination:**
- Body text on backgrounds
- Link text on backgrounds
- Button text on button backgrounds
- Icon colors on backgrounds
- All interactive states (hover, focus, active, disabled)

**Document failures:**
```
Issue: Insufficient contrast
Location: Secondary button text
Current: #888888 on #FFFFFF (2.9:1)
Required: 4.5:1 (WCAG AA)
Fix: Use #595959 on #FFFFFF (7.0:1)
```

### 2. Keyboard Navigation Test
**Simulate keyboard-only use:**

**Check:**
- Can reach all interactive elements with Tab
- Tab order is logical
- Enter/Space activates buttons
- Escape closes modals
- Arrow keys work (where appropriate)
- No keyboard traps

**Focus indicators:**
- Visible on all focusable elements
- Sufficient contrast (3:1)
- Not removed by CSS
- Clear enough to see

### 3. Screen Reader Review
**Test with:**
- NVDA (Windows, free)
- JAWS (Windows)
- VoiceOver (Mac/iOS)
- TalkBack (Android)

**Check:**
- Semantic HTML implied (headings, lists, tables)
- ARIA labels where needed
- Form labels associated
- Button purposes clear
- Link destinations clear
- Dynamic content announced
- Error messages announced

### 4. Touch Target Audit
**Measure all interactive elements:**

**Requirements:**
- Minimum 44×44px (WCAG Level AA)
- 48×48px recommended
- Adequate spacing between targets
- No overlapping hit areas

**Common violations:**
- Icon-only buttons too small
- Checkbox/radio too small
- Link text too small
- Close buttons too small

### 5. Content Structure Review
**Check hierarchy:**
- One H1 per page
- No skipped heading levels
- Logical nesting
- Meaningful headings

**Check lists:**
- Navigation = <nav> with list
- Lists of items = <ul>/<ol>
- Definition lists where appropriate

### 6. Alternative Text Audit
**For each image:**

**Informative images:**
- Descriptive alt text
- Context-dependent
- Concise but complete

**Decorative images:**
- Empty alt=""
- Or CSS background
- Not announced by screen readers

**Complex images:**
- Short alt + long description
- Chart data in table format
- Diagram explained in text

**Functional images (icons, buttons):**
- Describe function, not appearance
- "Delete item" not "Trash can icon"

### 7. Form Accessibility
**Every form input:**
- Has visible or aria-label
- Label properly associated (for/id)
- Required indicated
- Error messages specific
- Help text available
- Fieldsets for groups

**Validation:**
- Inline validation with care
- Don't validate on every keystroke
- Error messages near fields
- aria-invalid on error
- aria-describedby linking messages

## WCAG Conformance Levels

### Level A (Minimum)
Basic accessibility - must meet

### Level AA (Standard)
Enhanced accessibility - **target level**
- 4.5:1 text contrast
- 3:1 UI component contrast
- Resize text 200%
- No keyboard trap
- Multiple ways to find content

### Level AAA (Enhanced)
Highest accessibility - nice to have
- 7:1 text contrast
- 4.5:1 large text contrast
- No time limits
- Very clear focus

**Recommendation:** Target Level AA for all products

## Common Accessibility Issues

### Critical (Must Fix)
1. **No keyboard access**
   - Impact: Cannot use without mouse
   - Fix: Make all interactive elements keyboard accessible

2. **Insufficient contrast**
   - Impact: Text unreadable
   - Fix: Increase contrast to 4.5:1 minimum

3. **Missing form labels**
   - Impact: Screen readers can't identify inputs
   - Fix: Add visible labels or aria-label

4. **No focus indicators**
   - Impact: Can't see where you are
   - Fix: Add visible :focus styles (3:1 contrast)

### Important (High Priority)
5. **Touch targets too small**
   - Impact: Hard to tap accurately
   - Fix: Increase to 44×44px minimum

6. **Missing alt text**
   - Impact: Images not described
   - Fix: Add descriptive alt text

7. **Poor heading structure**
   - Impact: Hard to navigate
   - Fix: Use proper H1→H2→H3 hierarchy

### Medium Priority
8. **No skip link**
   - Impact: Must tab through navigation every page
   - Fix: Add "Skip to main content" link

9. **Inconsistent navigation**
   - Impact: Harder to learn interface
   - Fix: Keep navigation consistent

10. **Time limits**
    - Impact: Not enough time for some users
    - Fix: Remove or allow extension

## Accessibility Documentation

### Issue Report Format
```markdown
## Issue #[N]: [Title]

**WCAG Criterion:** [1.4.3, 2.1.1, etc.]
**Level:** [A, AA, AAA]
**Severity:** Critical / High / Medium / Low

**Location:** [Where in design]

**Issue:** [What's wrong]

**Impact:** [Who is affected and how]

**Current State:**
[Screenshot or description]

**Recommendation:**
[Specific fix with example]

**Success Criteria:**
[How to verify it's fixed]
```

### Example Issue
```markdown
## Issue #3: Insufficient Button Contrast

**WCAG:** 1.4.3 Contrast (Minimum)
**Level:** AA
**Severity:** Critical

**Location:** Primary CTA buttons throughout app

**Issue:** 
Button text (#888888) on button background (#FFFFFF) has contrast ratio of 2.9:1, below the required 4.5:1 for normal text.

**Impact:**
Users with low vision or color vision deficiencies cannot read button text. This affects the primary action on every page.

**Current State:**
[Screenshot showing low contrast button]
Text: #888888 on Background: #FFFFFF = 2.9:1

**Recommendation:**
Option 1: Darken text to #595959 (7.0:1)
Option 2: Add colored background, white text
  - Background: #0066CC, Text: #FFFFFF (7.5:1)

**Success Criteria:**
- All button text/background combinations meet 4.5:1 minimum
- Verified with contrast checker
- Tested in greyscale
```

## Testing Tools

**Automated:**
- axe DevTools (browser extension)
- WAVE (browser extension)
- Lighthouse (Chrome DevTools)
- Pa11y (command line)

**Manual:**
- Keyboard (Tab, Enter, Escape, Arrows)
- Screen reader (NVDA, JAWS, VoiceOver)
- Contrast checker (WebAIM)
- Color blind simulator (Stark, Color Oracle)

**Design tools:**
- Stark (Figma plugin)
- Able (Figma plugin)
- Contrast (Figma plugin)

## Best Practices

✅ **Do:**
- Test early and often
- Use automated and manual testing
- Test with real assistive technology
- Involve users with disabilities
- Make accessibility part of process
- Document decisions
- Train team
- Regular audits

❌ **Don't:**
- Rely only on automated tools (catch ~30%)
- Test only at the end
- Assume compliance without testing
- Remove focus indicators
- Use color alone to convey meaning
- Ignore keyboard users
- Treat as checklist only

## Deliverables
1. Accessibility audit report
2. Prioritized issue list
3. Remediation recommendations
4. WCAG compliance checklist
5. Training materials

Begin by running automated scans, then manual keyboard and screen reader testing.
