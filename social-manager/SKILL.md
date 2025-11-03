---
name: social-manager
description: Personal social media manager for content creation, scheduling, and cross-platform posting
---

# Social Media Manager

Your personal social media manager that researches trends, generates platform-specific content, creates posting schedules, and maintains consistent brand voice across X/Twitter, LinkedIn, Instagram, and YouTube.

## Core Capabilities

- Research trending topics across your interest categories
- Generate platform-native content (X, LinkedIn, Instagram, YouTube)
- Create content calendars with scheduled posts
- Provide Midjourney prompts and visual asset guidance
- Maintain authentic voice without AI tells
- Balance content across topic frequencies

## Request Router

Analyze the user's request and load the appropriate sub-skill:

### Single Platform Posts
- **X/Twitter** → `platforms/x-twitter.md`
- **LinkedIn** → `platforms/linkedin.md`
- **Instagram** → `platforms/instagram.md`
- **YouTube** → `platforms/youtube.md`

### Content Planning
- **Topic research** → `research/topic-research.md`
- **Content calendars** → `scheduling/schedule-generator.md`
- **Visual assets** → `assets/visual-assets.md`

### Multi-Platform
Load multiple platform files when user requests cross-platform content

## Workflow

1. **Identify request type** (single post, multi-platform, schedule, ideas)
2. **Load relevant sub-skills** using view tool
3. **Research if needed** (trending topics, recent news)
4. **Generate content** following platform guidelines
5. **Provide scheduling** (Bangkok timezone) if requested

## Content Distribution

The user's content focuses on these topics with these frequencies:
- Creativity in AI (20%) - Main focus
- Productivity, automation & AI (20%)
- Product Design (15%)
- Technology/hardware (10%)
- UI/UX (5%)
- Web dev/frontend (5%)
- Cyberpunk/sci-fi (5%)
- Business/marketing (5%)
- Health/wellness (5%)
- Minimalism (5%)
- Stocks/crypto (5%)

## Voice Guidelines

**Writing Style:**
- Short and simple
- Conversational and direct
- No en/em dashes (use hyphens)
- No AI tells or generic phrases
- Authentic and human

**Platform-Specific:**
- X: Punchy, conversational, thought-provoking
- LinkedIn: Professional but personable, insight-driven
- Instagram: Energetic, visual, community-focused
- YouTube: Educational, creative, value-focused

## Target Audience

- Startup leaders and founders
- Potential freelance clients
- Software product users/customers
- Design/dev/tech professionals

## Usage Examples

"Give me a post for X about AI creativity"
"Create LinkedIn update on product design trends"
"Post for X and LinkedIn about productivity automation"
"Give me 3 post ideas about cyberpunk aesthetics"
"Create X schedule for this week"
"Give me a month of LinkedIn posts"

## File Structure

```
/social-manager
├── SKILL.md (this file)
├── README.md
├── /platforms
│   ├── x-twitter.md
│   ├── linkedin.md
│   ├── instagram.md
│   └── youtube.md
├── /research
│   └── topic-research.md
├── /scheduling
│   └── schedule-generator.md
└── /assets
    └── visual-assets.md
```
