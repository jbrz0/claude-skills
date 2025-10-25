---
name: design-estimation
description: Estimate design work accurately with systematic task breakdown
category: Workflow & Process
tags: [estimation, planning, timeline, project-management, scope]
version: 1.0.0
---

# Design Estimation

Expert in estimating design work. Help designers break down projects, estimate effort accurately, and communicate timelines realistically to stakeholders.

## Task
Guide creation of realistic design estimates through systematic breakdown of work, consideration of variables, and communication of timelines with appropriate buffers.

## Why Estimation Matters

**Benefits:**
- Sets realistic expectations
- Enables planning
- Prevents overcommitment
- Builds trust
- Helps prioritize

**Challenges:**
- Many unknowns
- Iterative process
- Scope creep
- Dependencies
- Interruptions

## Estimation Approach

### 1. Break Down the Work

**Decompose project into:**
- Phases (Research → Design → Test)
- Deliverables (Flows, screens, specs)
- Tasks (Individual activities)

**Example breakdown:**
```
Mobile Checkout Redesign
├── Research (40 hours)
│   ├── User interviews (16h)
│   ├── Usability testing (12h)
│   ├── Analysis & synthesis (8h)
│   └── Presentation (4h)
├── Design (60 hours)
│   ├── User flows (8h)
│   ├── Wireframes (16h)
│   ├── High-fidelity design (24h)
│   ├── Responsive versions (8h)
│   └── Iterations (4h)
├── Testing (20 hours)
│   ├── Prototype creation (8h)
│   ├── User testing (8h)
│   └── Analysis (4h)
└── Handoff (12 hours)
    ├── Documentation (6h)
    ├── Design specs (4h)
    └── Developer support (2h)

Total: 132 hours = ~3.5 weeks
```

### 2. Estimate Each Task

**Use these units:**
- Hours (for small tasks)
- Days (for medium tasks)
- Weeks (for large phases)

**T-shirt sizing (rough estimates):**
- XS: 1-2 hours
- S: Half day
- M: 1 day
- L: 2-3 days
- XL: 1 week
- XXL: 2+ weeks

### 3. Consider Variables

**Factors affecting time:**

**Complexity:**
- Simple: Standard patterns
- Medium: Some custom work
- Complex: Novel solutions

**Fidelity:**
- Low-fi sketches: Faster
- Wireframes: Medium
- High-fi: Slower
- Polished: Slowest

**Scope:**
- Screens count
- States (default, error, loading, etc.)
- Responsive (mobile, tablet, desktop)
- Platforms (iOS, Android, web)

**Dependencies:**
- Waiting for decisions
- External resources
- Stakeholder availability

**Your experience:**
- Familiar domain: Faster
- New territory: Slower

**Team:**
- Solo: Full time allocation
- Collaboration: Coordination overhead

### 4. Add Buffers

**Why buffer:**
- Unknown unknowns
- Scope creep
- Iterations
- Feedback cycles
- Other responsibilities

**Buffer amounts:**
- Well-defined project: +20-30%
- Some unknowns: +30-50%
- Many unknowns: +50-100%

**Example:**
Base estimate: 100 hours
Buffer (30%): +30 hours
Total: 130 hours

### 5. Account for Other Work

**Your time isn't 100% project work:**
- Meetings (15-20%)
- Email/communication (10-15%)
- Other projects (varies)
- Team activities (5-10%)
- Learning/growth (5-10%)

**Available project hours:**
40 hour week × 60-70% = 24-28 hours actual project time

### 6. Communicate the Estimate

**Provide range, not single number:**
❌ "This will take exactly 10 days"
✅ "This will take 8-12 days, most likely 10"

**Explain assumptions:**
"This assumes we have content ready and one round of revisions"

**State confidence level:**
"High confidence" vs. "Rough estimate - many unknowns"

**Show your work:**
Share breakdown so they understand

## Estimation Methods

### Bottom-Up (Detailed)
**Process:**
1. List all tasks
2. Estimate each
3. Sum total

**When:** Well-defined projects

**Accuracy:** Higher

### Top-Down (Analogous)
**Process:**
1. Compare to similar past project
2. Adjust for differences

**When:** Quick estimate needed

**Accuracy:** Lower, but faster

### Three-Point Estimate
**Process:**
1. Best case: Everything goes perfectly
2. Most likely: Realistic scenario
3. Worst case: Murphy's Law

**Formula:** (Best + 4×Most Likely + Worst) / 6

**Example:**
- Best: 60 hours
- Most likely: 80 hours
- Worst: 120 hours
- Estimate: (60 + 4×80 + 120) / 6 = 87 hours

## Estimation Templates

### Task List Template
```
| Task | Complexity | Hours | Notes |
|------|------------|-------|-------|
| User research | M | 40 | 10 interviews |
| Wireframes | M | 20 | 8 key screens |
| Hi-fi design | H | 32 | 8 screens × 4h |
| Prototype | L | 8 | Interactive |
| Testing | M | 16 | 5 users |
| Iterations | ? | 12 | Buffer |
| Documentation | L | 6 | Handoff docs |
|------|------------|-------|-------|
| **Total** | | **134** | |
| **Buffer (25%)** | | **+34** | |
| **Grand Total** | | **168 hours** | **= 4-5 weeks** |
```

### Phase Estimate
```
Research Phase: 1.5-2 weeks
- User interviews
- Competitive analysis
- Synthesis

Design Phase: 3-4 weeks
- Ideation
- Wireframes
- High-fidelity designs
- Design system updates

Testing Phase: 1-2 weeks
- Prototype
- User testing
- Iterations

Handoff: 0.5-1 week
- Documentation
- Specs
- Developer support

Total: 6-9 weeks
Most likely: 7-8 weeks
```

## Scope Levels

### MVP (Minimum)
- Happy path only
- Core screens
- Desktop OR mobile
- One platform

**Estimate:** Baseline

### Standard
- Happy path + key edge cases
- All necessary screens
- Responsive (mobile + desktop)
- Primary platform

**Estimate:** Baseline × 1.5-2

### Comprehensive
- All user flows
- All edge cases
- All states
- Multi-platform
- Accessibility audit
- Design system documentation

**Estimate:** Baseline × 2-3

## Common Estimation Mistakes

❌ **Avoid:**
- Only estimating happy path
- Forgetting revisions
- Not accounting for meetings
- Being too precise (false confidence)
- Ignoring past experience
- Underestimating unknowns
- Promising what stakeholders want to hear
- No buffer
- Forgetting handoff time

✅ **Do:**
- Include all states and edge cases
- Plan for iterations
- Account for other responsibilities
- Give ranges
- Learn from past projects
- Ask questions to reduce unknowns
- Be realistic, not optimistic
- Add appropriate buffer
- Include documentation time

## Managing Estimates

### Track actual time:**
- Log what actually took
- Compare to estimates
- Learn patterns
- Improve future estimates

### Update as you learn:**
- New information emerges
- Scope changes
- Re-estimate and communicate

### Communicate changes:**
"We discovered X which adds Y time"
"Scope increased, new estimate is Z"

## Saying No (Or Not Yet)

**When timeline unrealistic:**
"To deliver quality work in that timeframe, we'd need to reduce scope to just [core features]."

"I can deliver X by then, or full scope by [realistic date]. Which is more important?"

"Let me show you the work involved and we can discuss trade-offs."

## Deliverables
1. Detailed task breakdown
2. Time estimates per task
3. Timeline with milestones
4. Assumptions documented
5. Risk factors noted

Begin by thoroughly understanding scope and breaking work into estimatable tasks.
