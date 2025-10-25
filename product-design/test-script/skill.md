# Test Script for Moderated Testing

Expert in writing test scripts for moderated usability tests. Help designers create structured scripts that elicit natural behavior while ensuring consistency across sessions.

## Task
Guide creation of test scripts that balance structure with flexibility, enabling moderators to gather rich insights while maintaining consistency.

## Script Components

### 1. Introduction (5 min)
**Welcome and rapport:**
"Hi [Name], thanks for joining. I'm [Your name], and I'll be guiding today's session."

**Purpose:**
"We're testing [product/feature] to understand how people use it and where we can improve. Your honest feedback helps us make it better."

**Set expectations:**
- Duration (45-60 min typical)
- Think-aloud protocol
- No wrong answers
- You're testing the product, not being tested
- OK to criticize
- Can stop anytime

**Consent:**
- Recording permission
- Confidentiality
- How data will be used

**Questions?**
"Any questions before we start?"

### 2. Background Questions (5-10 min)
**Warm-up and context:**
- Easy, non-threatening questions
- Build rapport
- Understand their context
- Assess experience level

**Example questions:**
- "Tell me about your current role"
- "How do you typically handle [task related to product]?"
- "What tools do you currently use for this?"
- "How often do you [activity]?"

### 3. Main Tasks (30-40 min)
**For each task:**

**Scenario setup:**
"Imagine you're [scenario]. You want to [goal]. Show me how you would do that."

**Task introduction:**
- Context/scenario
- Goal (not steps)
- Starting point
- Success criteria

**Observation:**
- Let them work
- Minimal intervention
- Note behaviors
- Take notes

**Probing (as needed):**
- "What are you thinking?"
- "What do you expect to happen?"
- "Why did you click that?"
- "Tell me more about that"

**After each task:**
- "How easy or difficult was that?" (1-5 scale)
- "What, if anything, was confusing?"
- "How would you expect that to work?"

### 4. Post-Task Questions (5-10 min)
**Overall impressions:**
- "What did you think overall?"
- "What worked well?"
- "What was frustrating?"
- "What would you change?"
- "Would you use this? Why or why not?"

**Comparative:**
- "How does this compare to [competitor/current tool]?"
- "What does this do better?"
- "What does [other tool] do better?"

**Satisfaction:**
- System Usability Scale (SUS) questionnaire
- Net Promoter Score
- Custom rating questions

### 5. Wrap-up (2-3 min)
**Final questions:**
"Is there anything else you'd like to share?"
"What haven't I asked that I should have?"

**Thank you:**
"Thank you so much for your time and insights. This is incredibly helpful."

**Next steps:**
- How feedback will be used
- Timeline
- Incentive distribution
- Contact info if follow-up needed

## Task Writing Guidelines

### Good Task Characteristics:

**Realistic scenario:**
✅ "You're planning a trip and want to find a hotel near the beach..."
❌ "Click on the 'Hotels' button"

**Clear goal:**
✅ "Find a hotel under $150/night"
❌ "Browse around the site"

**Open-ended approach:**
✅ "Show me how you would do that"
❌ "Use the search box in the top right"

**Natural language:**
✅ "You want to save this for later"
❌ "Add this item to your favorites list"

### Task Template:

```
Task [N]: [Task name]

Scenario:
"Imagine you're [context]. You want to [goal] because [motivation]."

Starting point:
[Where they begin - URL or app screen]

Task:
"Show me how you would [action to complete goal]."

Success criteria (for moderator):
- [ ] User navigates to X
- [ ] User completes Y
- [ ] User finds Z

Time limit: [X minutes] (if applicable)

If they get stuck:
[Hint 1 - after 2 min]
[Hint 2 - after 4 min]
```

### Example Tasks:

**Task 1: Find and Book Hotel**
```
Scenario:
"You're planning a weekend trip to San Francisco next month. You want to find a hotel near Fisherman's Wharf that costs under $150 per night."

Starting point:
Homepage (www.example.com)

Task:
"Show me how you would find and book a hotel for this trip."

Success criteria:
- [ ] Uses search with location and dates
- [ ] Applies price filter
- [ ] Sorts/filters results
- [ ] Selects a hotel
- [ ] Proceeds to booking

Time limit: 10 minutes

If stuck:
- 2 min: "What would you expect to do first?"
- 5 min: "What information do you need to provide?"
```

## Think-Aloud Protocol

### Instructions to participant:

"As you work through the tasks, please think out loud - tell me what you're thinking, what you're looking for, what you expect to happen. It might feel awkward at first, but it really helps me understand your experience."

### Example:
"So I'm clicking this button because I'm looking for... wait, that's not what I expected. Let me try... hmm, this is confusing..."

### If they go silent:
"What are you thinking right now?"
"Talk me through what you're doing"
"What are you looking for?"

## Moderator Notes

### Do:
✅ Stay neutral (no leading)
✅ Encourage thinking aloud
✅ Probe for reasoning
✅ Note non-verbal cues
✅ Let them struggle (briefly)
✅ Manage time
✅ Show empathy

### Don't:
❌ Lead or help
❌ Defend the design
❌ Interrupt
❌ Show judgment
❌ Let them fail endlessly
❌ Rush them
❌ Make it about you

### Neutral prompts:
- "What are you thinking?"
- "Tell me more"
- "Interesting, why's that?"
- "What would you expect?"
- "How would you describe this?"

### Non-leading helps:
If really stuck after time limit:
- "What would you do if I weren't here?"
- "Where would you expect to find that?"
- Last resort: "Try clicking [area] and see what happens"

## Sample Complete Script

```markdown
# Usability Test Script: Mobile Banking App

## Pre-Session Setup
- [ ] Prototype link ready
- [ ] Recording started
- [ ] Consent form signed
- [ ] Participant ID logged

## Introduction (5 min)

**Welcome:**
"Hi [Name], I'm [Your name]. Thanks for joining today. How are you?"

**Purpose:**
"We're testing a new mobile banking app to see how people use it and where we can make improvements. Your honest feedback - both positive and negative - helps us make it better for everyone."

**Explain think-aloud:**
"As you go through tasks, please think out loud - tell me what you're thinking, what you're looking for, what confuses you. It might feel weird at first, but it really helps me understand your experience."

**Set expectations:**
- About 45 minutes
- No right or wrong answers
- You're testing the app, not being tested
- Feel free to be critical - you won't hurt my feelings!
- OK to quit anytime
- Any questions OK

**Consent:**
"I'd like to record this session so I can review it later. Your name won't be attached to any reports. Is that OK?"

[Start recording]

**Questions?**

## Background (5 min)

"Before we look at the app, I'd like to learn a bit about you."

1. "Tell me about your current mobile banking habits"
   - How often?
   - What do you use it for?
   - What app(s)?

2. "What do you like about your current banking app?"

3. "What frustrates you about it?"

4. "On a scale of 1-5, how tech-savvy would you say you are?"

## Tasks (30 min)

"Great, now let's look at the new app. Remember to think aloud as you go."

### Task 1: Check Balance (Baseline - 3 min)

**Scenario:**
"You want to quickly check your checking account balance."

**Task:**
"Show me how you would do that."

**Success:** Navigates to accounts, views checking balance

**After task:**
- "How easy was that? 1-5"
- "What did you think?"

### Task 2: Transfer Money (Primary - 8 min)

**Scenario:**
"You need to transfer $500 from your checking account to your savings account."

**Task:**
"Show me how you would do that using this app."

**Success:**
- Finds transfer feature
- Selects accounts correctly  
- Enters amount
- Confirms transfer

**If stuck (after 3 min):**
"Where would you expect to find that option?"

**After task:**
- "How easy was that? 1-5"
- "What was clear?"
- "What was confusing?"
- "Did anything surprise you?"

### Task 3: Find Transaction (Secondary - 5 min)

**Scenario:**
"Last week you paid your electric bill for $87.32. You want to find that transaction to confirm it went through."

**Task:**
"Show me how you would find that transaction."

**Success:**
- Navigates to transaction history
- Searches or filters
- Locates transaction

**After task:**
- "How easy was that? 1-5"
- "How would you improve the search?"

## Post-Tasks (5 min)

**Overall:**
1. "Overall, what did you think of the app?"
2. "What worked really well?"
3. "What was most frustrating?"
4. "If you could change one thing, what would it be?"

**Comparative:**
5. "How does this compare to your current banking app?"
6. "Would you use this app? Why or why not?"

**SUS Questionnaire:**
[Administer System Usability Scale]

## Wrap-up (2 min)

"We're all done. Thank you so much for your time and honest feedback. This is really valuable."

"Is there anything else you'd like to share?"

**Next steps:**
"We'll use this feedback to improve the design. Your gift card should arrive by email within 24 hours."

**Questions?**

"Thanks again!"

[Stop recording]

## Post-Session
- [ ] Save recording
- [ ] Clean up notes
- [ ] Rate task success (0-4 scale)
- [ ] Note key issues
- [ ] Highlight quotes
```

## Best Practices

✅ **Do:**
- Pilot test script
- Time each section
- Have backup tasks
- Take good notes
- Stay on schedule
- Build rapport
- Be flexible

❌ **Don't:**
- Read robotically
- Skip warm-up
- Lead participants
- Show bias
- Argue or defend
- Go way over time

## Deliverables
1. Complete test script
2. Task cards (for moderator)
3. Consent form
4. Participant screener
5. Note-taking template

Begin by defining research goals and key tasks to test.
