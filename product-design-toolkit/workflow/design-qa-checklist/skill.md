---
name: design-qa-checklist
description: Comprehensive QA checklist for design review before handoff
category: Workflow & Process
tags: [qa, quality-assurance, checklist, review, handoff]
version: 1.0.0
---

# Design QA Checklist

Expert in design quality assurance. Help designers create comprehensive checklists to review designs before handoff, ensuring nothing is missed.

## Task
Guide creation and use of design QA checklists that catch issues before development, ensuring complete, consistent, high-quality deliverables.

## Why Design QA Matters

**Prevents:**
- Missing states
- Inconsistencies
- Accessibility issues
- Poor handoffs
- Developer questions
- Rework

**Ensures:**
- Completeness
- Quality
- Consistency
- Professionalism
- Smooth handoff

## Master Design QA Checklist

### ✅ Completeness

**All screens designed:**
- [ ] Every screen in user flow
- [ ] All platforms (mobile, desktop, tablet)
- [ ] All device sizes
- [ ] Key breakpoints

**All states covered:**
- [ ] Default/initial state
- [ ] Hover (desktop)
- [ ] Focus (keyboard)
- [ ] Active/pressed
- [ ] Selected/active
- [ ] Loading
- [ ] Success
- [ ] Error
- [ ] Disabled
- [ ] Empty state

**Edge cases:**
- [ ] Very long content
- [ ] Very short content
- [ ] No content
- [ ] Maximum items
- [ ] Minimum items
- [ ] Special characters
- [ ] Different languages

### ✅ Visual Design

**Typography:**
- [ ] All text styles defined in design system
- [ ] Font sizes appropriate (16px+ for body)
- [ ] Line heights set (1.5+ for body)
- [ ] Hierarchy clear
- [ ] Consistent font usage
- [ ] Real content (not Lorem Ipsum)

**Color:**
- [ ] All colors from design tokens
- [ ] Sufficient contrast (4.5:1 text, 3:1 UI)
- [ ] Accessible in dark mode (if applicable)
- [ ] Not relying on color alone
- [ ] Consistent color usage

**Spacing:**
- [ ] Using consistent spacing scale
- [ ] Adequate padding
- [ ] Clear margins
- [ ] Proper alignment
- [ ] Breathing room

**Layout:**
- [ ] Grids used consistently
- [ ] Alignment clean
- [ ] Hierarchy clear
- [ ] Balanced composition
- [ ] Responsive behavior defined

### ✅ Components

**Usage:**
- [ ] Using design system components
- [ ] No detached components (or documented why)
- [ ] Props configured correctly
- [ ] Variants used appropriately

**Consistency:**
- [ ] Same component used for same purpose
- [ ] Similar elements look similar
- [ ] Buttons consistent
- [ ] Form fields consistent

**States:**
- [ ] All component states designed
- [ ] Hover effects defined
- [ ] Focus indicators visible
- [ ] Disabled states clear

### ✅ Interactions

**Behaviors defined:**
- [ ] Click/tap actions specified
- [ ] Hover behaviors (desktop)
- [ ] Focus behaviors (keyboard)
- [ ] Transitions/animations detailed
- [ ] Loading states shown

**Feedback:**
- [ ] User gets feedback after actions
- [ ] Loading indicators present
- [ ] Success confirmation shown
- [ ] Errors clearly communicated

**Navigation:**
- [ ] Clear paths forward
- [ ] Back/cancel options
- [ ] Breadcrumbs (if needed)
- [ ] Current location indicated

### ✅ Content

**Copy:**
- [ ] All copy written (no placeholder)
- [ ] Tone consistent
- [ ] Clear and concise
- [ ] Error messages helpful
- [ ] Button labels action-oriented

**Images:**
- [ ] Real images (not FPO)
- [ ] Proper resolution (@2x, @3x)
- [ ] Alt text specified
- [ ] Image sources documented

**Icons:**
- [ ] All icons from set
- [ ] Consistent style
- [ ] Appropriate size
- [ ] Meaningful (not decorative only)

### ✅ Responsive Design

**Breakpoints:**
- [ ] Mobile (320-767px)
- [ ] Tablet (768-1023px)
- [ ] Desktop (1024px+)
- [ ] Large desktop (1440px+)

**Behavior:**
- [ ] Layout adapts appropriately
- [ ] Content reflows well
- [ ] Images scale/crop correctly
- [ ] Navigation appropriate per size
- [ ] Touch targets adequate (44px+)

**Testing:**
- [ ] Viewed at actual sizes
- [ ] Tested reflow
- [ ] Checked extremes (320px, 2560px)

### ✅ Accessibility

**Keyboard:**
- [ ] All interactive elements reachable
- [ ] Logical tab order
- [ ] Focus indicators visible (3:1 contrast)
- [ ] No keyboard traps
- [ ] Enter/Space work on buttons

**Screen reader:**
- [ ] Alt text for images
- [ ] Labels for form inputs
- [ ] Heading hierarchy (H1→H2→H3)
- [ ] ARIA labels where needed
- [ ] Semantic structure

**Visual:**
- [ ] Text contrast ≥ 4.5:1
- [ ] UI elements contrast ≥ 3:1
- [ ] Touch targets ≥ 44×44px
- [ ] Not using color alone
- [ ] Works in grayscale

**Motion:**
- [ ] No auto-playing video with sound
- [ ] Animations can be paused
- [ ] Respects prefers-reduced-motion
- [ ] No flashing (>3 times/sec)

### ✅ Documentation

**Annotations:**
- [ ] Key interactions noted
- [ ] Edge cases explained
- [ ] Complex behaviors detailed
- [ ] Measurement callouts

**Specs:**
- [ ] Spacing documented
- [ ] Colors specified
- [ ] Typography defined
- [ ] Component props listed

**Flows:**
- [ ] User flows created
- [ ] Decision points shown
- [ ] Error paths included
- [ ] Success paths clear

**Handoff notes:**
- [ ] Technical constraints noted
- [ ] Priority/phasing indicated
- [ ] Known issues flagged
- [ ] Questions answered

### ✅ Organization

**Files:**
- [ ] Logical page structure
- [ ] Clear naming
- [ ] Grouped appropriately
- [ ] No orphaned frames

**Layers:**
- [ ] Named clearly
- [ ] Organized logically
- [ ] Grouped properly
- [ ] No hidden elements (unintentionally)

**Components:**
- [ ] Published to library
- [ ] Variants organized
- [ ] Props configured
- [ ] Examples shown

**Styles:**
- [ ] All colors as styles
- [ ] All text as styles
- [ ] No local overrides (or documented)
- [ ] Organized by category

### ✅ Cross-Platform Consistency

**iOS & Android:**
- [ ] Platform patterns followed
- [ ] Native components used
- [ ] Gestures appropriate
- [ ] Terminology correct

**Web & Mobile:**
- [ ] Consistent experience
- [ ] Appropriate for platform
- [ ] Feature parity (or documented)

### ✅ Performance Considerations

**Images:**
- [ ] Optimized file sizes
- [ ] Appropriate formats
- [ ] Lazy loading planned

**Content:**
- [ ] Pagination for long lists
- [ ] Infinite scroll considered
- [ ] Load time acceptable

**Animations:**
- [ ] GPU-accelerated (transform, opacity)
- [ ] Not overused
- [ ] Performant on low-end devices

## QA Process

### Self-Review

**Before handoff:**
1. Go through checklist
2. View at actual sizes
3. Click through prototype
4. Test keyboard navigation
5. Run contrast checker
6. Check in grayscale

### Peer Review

**Ask colleague:**
- Review against checklist
- Find inconsistencies
- Test interactions
- Question decisions

### Stakeholder Review

**Present to:**
- Product (feature completeness)
- Engineering (feasibility)
- Accessibility (compliance)
- Content (copy)

### Pre-Development Check

**Final pass:**
- [ ] All feedback addressed
- [ ] Designs approved
- [ ] Specs complete
- [ ] Questions answered
- [ ] Ready for dev

## QA Documentation

### Issue Log

```markdown
| Issue | Severity | Status | Owner |
|-------|----------|--------|-------|
| Missing error state for form | High | Fixed | Designer |
| Low contrast on disabled button | Medium | Fixed | Designer |
| No alt text on hero image | High | Fixed | Content |
```

**Severity:**
- **Critical:** Blocks dev, must fix
- **High:** Should fix before handoff
- **Medium:** Fix soon
- **Low:** Nice to have

## Platform-Specific Checklists

### Mobile App
- [ ] All OS-specific patterns followed
- [ ] Status bar designed
- [ ] Safe areas respected
- [ ] Gestures intuitive
- [ ] Offline state designed
- [ ] Push notifications designed

### Web App
- [ ] Browser compatibility noted
- [ ] URL structure defined
- [ ] SEO considerations
- [ ] Print styles (if needed)
- [ ] Share/og:image

### Desktop App
- [ ] Window states (min, max, full)
- [ ] Menu bar
- [ ] Keyboard shortcuts
- [ ] Multi-window behavior

## Best Practices

✅ **Do:**
- Use checklist every time
- Review early and often
- Get peer feedback
- Test accessibility
- Document issues
- Fix before handoff
- Learn from mistakes

❌ **Don't:**
- Skip QA to save time
- Only check happy path
- Ignore accessibility
- Leave placeholders
- Hand off incomplete work
- Assume developers will fix

## Deliverables
1. Completed QA checklist
2. Issue log (if any)
3. Final reviewed designs
4. Sign-off from stakeholders

Begin QA early, review throughout design process, and do final check before handoff.
