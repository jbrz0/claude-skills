# Health Toolkit

Comprehensive health optimization system for Claude with specialized expertise in nutrition, fitness training, sleep optimization, and migraine management.

## Overview

The Health Toolkit is a modular skill system that provides evidence-based guidance across four core health domains:

- **Nutrition System:** Calorie/macro calculations, meal planning, body recomposition
- **Fitness Protocol:** Training program design, progressive overload, exercise technique
- **Sleep Optimization:** Sleep quality, circadian rhythm, recovery optimization
- **Migraine Management:** Trigger tracking, prevention strategies, treatment protocols

Each sub-skill is comprehensive (10k+ words) and can be used independently or integrated together for complete health optimization.

## File Structure

```
health-toolkit/
├── SKILL.md                           # Main router file
├── README.md                          # This file
├── nutrition/
│   └── nutrition-system.md           # Complete nutrition guide
├── fitness/
│   └── fitness-protocol.md           # Training program design
├── sleep/
│   └── sleep-optimization.md         # Sleep quality improvement
└── migraine/
    └── migraine-management.md        # Migraine prevention & treatment
```

## Installation

1. Copy the entire `health-toolkit` directory to your Claude skills folder
2. Claude will automatically detect the SKILL.md router file
3. Reference by name: "Use the health-toolkit" or specific sub-skills

## Usage

### Basic Usage

Simply tell Claude what you need help with:

```
"Help me calculate my calorie needs and set macros"
→ Routes to nutrition-system.md

"Design a 4-day strength training program"
→ Routes to fitness-protocol.md

"I'm not sleeping well, help me fix it"
→ Routes to sleep-optimization.md

"Help me identify my migraine triggers"
→ Routes to migraine-management.md
```

### Multi-Domain Optimization

For comprehensive health work:

```
"Create a complete plan for muscle gain with nutrition and training"
→ Integrates nutrition-system + fitness-protocol

"My migraines might be related to sleep, help me investigate"
→ Integrates migraine-management + sleep-optimization

"Help me optimize all areas of my health"
→ Uses all sub-skills systematically
```

### Direct Sub-Skill Reference

You can also directly reference specific skills:

```
"Using the nutrition system, calculate my cutting calories"
"Show me the fitness protocol for hypertrophy training"
"Walk me through the sleep optimization environment setup"
"Use the migraine management system to analyze my triggers"
```

## Key Features

### Evidence-Based
- All recommendations backed by research
- No pseudoscience or unproven hacks
- Citations and rationale provided
- Acknowledges when evidence is limited

### Practical and Actionable
- Step-by-step implementation guides
- Real-world examples and calculations
- Decision frameworks for common scenarios
- Troubleshooting for common mistakes

### Personalized
- Calculations based on your stats
- Adjustable for preferences and constraints
- Individual variation acknowledged
- Systematic self-experimentation approach

### Integrated
- Cross-references between sub-skills
- Shows how areas interact
- Prevents contradictory advice
- Systems thinking approach

## Sub-Skill Summaries

### Nutrition System (~11k words)

**Core Content:**
- TDEE calculation and calorie targets
- Macro programming (protein/carbs/fats)
- Meal planning strategies
- Food tracking methods
- Cutting vs bulking protocols
- Supplement guidance

**Best For:**
- Body recomposition goals
- Flexible dieting approach
- Evidence-based nutrition
- Sustainable eating habits

### Fitness Protocol (~11k words)

**Core Content:**
- Training program design
- Progressive overload principles
- Exercise selection and technique
- Recovery and deload strategies
- Periodization frameworks
- Injury prevention

**Best For:**
- Strength training programs
- Hypertrophy optimization
- Athletic performance
- Long-term progression

### Sleep Optimization (~11k words)

**Core Content:**
- Sleep quality improvement
- Circadian rhythm optimization
- Environment setup (light/temp/noise)
- Sleep hygiene protocols
- Supplement strategies
- Fixing insomnia

**Best For:**
- Poor sleep quality
- Inconsistent schedule
- Recovery optimization
- Energy and performance

### Migraine Management (~11k words)

**Core Content:**
- Trigger identification and tracking
- Prevention strategies (lifestyle + medication)
- Acute treatment protocols
- Special situations (menstrual, chronic, etc.)
- Working with doctors
- Pattern analysis

**Best For:**
- Frequent migraines (4+/month)
- Understanding triggers
- Prevention optimization
- Treatment effectiveness

## Integration Examples

### Example 1: Muscle Gain
**Goal:** Gain muscle and strength

**Sub-skills used:**
1. Nutrition System: Calculate surplus calories, set high protein macros
2. Fitness Protocol: Design progressive strength program
3. Sleep Optimization: Ensure adequate recovery (8+ hours)

**Integration points:**
- Nutrition surplus supports training volume
- Sleep enables muscle recovery and growth
- Training drives adaptation that nutrition supports

### Example 2: Migraine Reduction
**Goal:** Reduce migraine frequency

**Sub-skills used:**
1. Migraine Management: Identify triggers, prevention strategies
2. Sleep Optimization: Fix irregular schedule (major trigger)
3. Nutrition System: Regular meal timing, identify food triggers

**Integration points:**
- Sleep irregularity = common trigger
- Skipping meals = blood sugar trigger
- Consistent lifestyle = key to prevention

### Example 3: Fat Loss
**Goal:** Lose fat while maintaining muscle

**Sub-skills used:**
1. Nutrition System: Calculate deficit, set high protein
2. Fitness Protocol: Maintain strength training during deficit
3. Sleep Optimization: Manage hunger hormones, recovery

**Integration points:**
- Deficit from nutrition, muscle preservation from training
- Sleep affects hunger hormones and adherence
- All three must align for success

## When to Use vs When to See a Doctor

### Use This Skill For:
- General health optimization
- Evidence-based guidance
- Creating sustainable systems
- Understanding principles
- Self-experimentation frameworks
- Tracking and analysis

### See a Doctor For:
- Medical diagnoses
- Prescription medications
- Serious health conditions
- Persistent issues despite interventions
- Pregnancy or specific medical situations
- Anything requiring medical expertise

**This skill provides education and frameworks, not medical advice.**

## Philosophy

### Core Principles

**1. Foundations First**
- Sleep and basic nutrition before advanced tactics
- Master basics before adding complexity
- 80% results from 20% of interventions

**2. Sustainability Over Perfection**
- Systems you can maintain long-term
- Adherence beats optimal but unsustainable
- Progress over perfection

**3. Individual Variation**
- No one-size-fits-all
- Systematic self-experimentation required
- Track, assess, adjust

**4. Evidence-Based**
- Research-backed recommendations
- Acknowledges uncertainty
- Updates with new evidence

**5. Integration**
- Health areas interact
- Systems thinking
- Avoid siloed optimization

## Development and Updates

**Version:** 1.0.0

**Created:** October 2025

**Maintenance:**
- Evidence-based content, updated as research evolves
- Modular design allows independent sub-skill updates
- Open to feedback and improvements

## Contributing

Suggestions for improvements:
- Additional sub-skills (stress management, mental health, etc.)
- More integration examples
- Updated research and protocols
- User experience enhancements

## License

For personal use with Claude skills system.

## Acknowledgments

Built on principles from:
- Exercise science and strength training research
- Sports nutrition and body composition studies
- Sleep research and circadian biology
- Headache and migraine neurology

Evidence-based, practical, and designed for real-world application.

---

## Quick Start

1. **Assess:** Where are you now? What's your biggest gap?
2. **Choose:** Pick the sub-skill(s) that address your priority
3. **Implement:** Follow the specific protocols and frameworks
4. **Track:** Measure progress and patterns
5. **Adjust:** Refine based on your individual response
6. **Integrate:** Connect multiple areas as you advance

Tell Claude what you want to optimize, and the Health Toolkit will guide you there.