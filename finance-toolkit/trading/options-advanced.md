---
name: options-advanced
description: Advanced options strategies - butterflies, condors, spreads, defined-risk trades
category: Options Trading
tags: [options, butterfly, condor, spreads, iron-condor, defined-risk, advanced]
version: 1.0.0
---

# Advanced Options Strategies

Expert in advanced options strategies including butterflies, iron condors, vertical spreads, and other defined-risk trades. Help with setup, management, and risk-defined income generation.

## Your Advanced Trading Context

**Trading profile:**
- Account size: $X
- Risk per trade: $X or X%
- Preferred strategies: [BWB, IC, other]
- Target ROI per trade: X%
- Time commitment: [Active or passive management]

**Strategy preferences:**
- Broken wing butterfly (BWB): Yes/No
- Iron condor (IC): Yes/No
- Credit spreads: Yes/No
- Debit spreads: Yes/No
- Calendars: Yes/No

**Market assumptions:**
- Directional bias: Bullish/Bearish/Neutral
- Volatility outlook: Increasing/Decreasing/Stable
- Timeframe: Short-term/Medium-term/Long-term

## Strategy Overview

### Comparison Matrix
```
Strategy          | Risk      | Reward    | Best Market      | Complexity
------------------|-----------|-----------|------------------|------------
Iron Condor       | Defined   | Limited   | Low volatility   | Medium
Butterfly         | Defined   | Limited   | Pin to strike    | Medium
Broken Wing Fly   | Defined   | Limited   | Directional+pin  | High
Credit Spread     | Defined   | Limited   | Directional      | Low
Debit Spread      | Defined   | Limited   | Strong direction | Low
Calendar Spread   | Defined   | Limited   | Neutral/theta    | Medium
```

## Iron Condor

### What It Is

**Structure:**
- Sell OTM call spread (above current price)
- Sell OTM put spread (below current price)
- Collect premium from both sides
- Profit if stock stays in range

**Profit zone:**
```
     Short Put Strike -------- Short Call Strike
     [$95]                            [$105]
           [====PROFIT ZONE====]
Stock must stay between these strikes
```

**Risk profile:**
- Max profit: Premium collected
- Max loss: Wing width - Premium
- Defined risk both sides

### Setup Example
```markdown
## SPY Iron Condor

**Underlying:** SPY at $420

**Put side:**
- Buy $400 put
- Sell $405 put
- $5 wide spread
- Credit: $1.50

**Call side:**
- Sell $435 call
- Buy $440 call
- $5 wide spread
- Credit: $1.50

**Total credit:** $3.00 ($300 per IC)

**Risk/Reward:**
- Max profit: $300 (if SPY between $405-435 at expiration)
- Max loss: $200 ($500 wing - $300 credit)
- Breakevens: $402 and $438
- Profit zone: 33 points wide

**Return on risk:** $300 profit / $200 risk = 150% ROC if max profit
```

### Strike Selection for Iron Condor

**Standard: 0.16 delta on short strikes**
- Roughly 16% chance each side gets tested
- ~68% chance of profit (within 1 standard deviation)

**Width of profit zone:**
- Narrow (<15 points on SPY): Higher premium, higher risk
- Medium (20-30 points): Balanced
- Wide (>40 points): Lower premium, safer

**Wing width (spread size):**
- $5 wide: Standard, good risk/reward
- $10 wide: More capital required, less ROC
- $2-3 wide: Less capital, more risk

**DTE (Days to Expiration):**
- 30-45 DTE typical
- Manage at 21 DTE or 50% profit

### Management Rules

**Winning ICs:**
- Close at 50% max profit (keep $150 if collected $300)
- Close at 21 DTE if still in profit zone
- Roll both sides out if <7 DTE and near strikes

**Challenged ICs:**

**One side tested (stock moved to/through short strike):**
```
Stock moved up, threatening call side
Options:
1. Close entire IC (take loss)
2. Roll tested side out/up for credit
3. Close untested side, manage remaining as spread
4. Do nothing, hope for reversal (risky)

Recommendation: Roll tested side if can collect credit and stock not accelerating
```

**Both sides tested (high volatility event):**
```
Rare but possible (stock whipsawed)
Result: Both sides near max loss
Action: Close entire position, take loss
Lesson: Don't trade through earnings
```

### Iron Condor Best Practices

✅ **Do:**
- Trade high IV rank underlyings (>50th percentile)
- Use liquid underlyings (SPY, QQQ, IWM)
- Size positions appropriately (risk 2-5% per IC)
- Close at 50% profit (don't be greedy)
- Manage at 21 DTE
- Avoid earnings

❌ **Don't:**
- Trade low IV (not enough premium)
- Use illiquid stocks (can't exit)
- Over-leverage (blow up account)
- Let winners become losers (take profit!)
- Hold to expiration (pin risk)
- Trade through earnings (volatility spike)

## Butterfly Spread

### What It Is

**Structure:**
- Buy 1 OTM put/call
- Sell 2 ATM puts/calls
- Buy 1 further OTM put/call
- Net debit or credit (usually debit)

**Profit diagram:**
```
         /\
        /  \
       /    \
      /      \
     /        \
    /          \
-----------------
  Lower  ATM  Upper

Max profit at ATM strike
Wings define max loss
```

**Goal:** Stock pins to middle (ATM) strike

### Regular Butterfly Example
```markdown
## Call Butterfly on AAPL

**Underlying:** AAPL at $180

**Structure:**
- Buy 1 AAPL $175 call @ $7.00
- Sell 2 AAPL $180 calls @ $4.50 each
- Buy 1 AAPL $185 call @ $2.50
- Net debit: $0.50 ($50 per butterfly)

**Risk/Reward:**
- Max profit: $450 (if AAPL exactly $180 at expiration)
- Max loss: $50 (debit paid)
- Risk/Reward: $50 risk for $450 potential = 9:1
- Breakevens: $175.50 and $184.50

**Width:** $5 wings (common on stocks)

**When to use:**
- Neutral outlook (expect little movement)
- Low volatility expected
- High win rate if within range
```

### Broken Wing Butterfly (BWB)

**Modification:** Skewed risk to one side

**Structure (bearish BWB):**
```
Buy $95 put
Sell 2x $100 puts
Buy $110 put  <- Wing is wider here (10 points vs 5)

Benefits:
- Can collect credit instead of debit
- Directional bias (slightly bearish OK)
- Still defined risk

Risk:
- Max loss if stock moves to skewed wing
- But collected credit offsets
```

### BWB Example
```markdown
## SPY Broken Wing Butterfly (Bearish)

**Underlying:** SPY at $420

**Structure:**
- Buy 1 SPY $410 put
- Sell 2 SPY $415 puts
- Buy 1 SPY $430 put (15 points wide instead of 5)
- Net credit: $1.00 ($100 per BWB)

**Risk/Reward:**
- Max profit: $600 (if SPY at $415)
- Max loss: $400 (if SPY rallies to $430+)
- Profit if SPY between $411-429
- Wide profit zone!

**Directional bias:** Slightly bearish to neutral OK
**Why BWB?** More forgiving than regular butterfly

**Management:**
- Close at 50% of max profit
- Roll if stock threatening wide wing
- Safer than regular butterfly
```

### Butterfly Management

**Target exit: 25-50% of max profit**
- Butterflies need precision (stock to pin)
- Don't wait for max profit (rarely happens)
- Take profit when available

**Adjustments:**
```
Stock moving away from center:
- Let it expire (small loss)
- Close early (cut loss)
- Roll to new center (follow stock)

Stock approaching center (near max profit):
- Close early (take 50%+ profit)
- Don't wait for expiration (risk reversal)
```

## Credit Spreads

### Bull Put Spread

**Structure:**
- Sell OTM put (higher strike)
- Buy further OTM put (lower strike, protection)
- Net credit
- Bullish trade

**Example:**
```markdown
## Bull Put Spread on MSFT

**Underlying:** MSFT at $380

**Structure:**
- Sell $375 put @ $3.00
- Buy $370 put @ $1.50
- Net credit: $1.50 ($150 per spread)

**Risk/Reward:**
- Max profit: $150 (if MSFT above $375)
- Max loss: $350 ($500 spread - $150 credit)
- Breakeven: $373.50
- Return on risk: 43% ($150 / $350)

**Thesis:** MSFT stays above $375 (support level)

**Management:**
- Close at 50% profit ($75)
- Close/roll if stock breaks below $375
- Max hold to 21 DTE
```

### Bear Call Spread

**Structure:**
- Sell OTM call (lower strike)
- Buy further OTM call (higher strike, protection)
- Net credit
- Bearish trade

**Example:**
```markdown
## Bear Call Spread on TSLA

**Underlying:** TSLA at $230

**Structure:**
- Sell $240 call @ $4.00
- Buy $245 call @ $2.00
- Net credit: $2.00 ($200 per spread)

**Risk/Reward:**
- Max profit: $200 (if TSLA below $240)
- Max loss: $300 ($500 spread - $200 credit)
- Breakeven: $242
- Return on risk: 67%

**Thesis:** TSLA resistance at $240, stays below

**Management:**
- Close at 50% profit
- Roll up/out if stock breaks above $240
- Don't let it go to max loss
```

### Credit Spread Selection

**Strike selection:**
- Short strike: 0.25-0.35 delta (25-35% OTM)
- Spread width: $5-10 typical
- Premium target: 1/3 of spread width

**Example:**
```
$5 spread: Target $1.50-2.00 credit (30-40%)
$10 spread: Target $3.00-4.00 credit (30-40%)
```

**DTE:** 30-45 days typical

**Position sizing:**
- Risk: 2-5% of account per spread
- Max loss is defined (spread width - credit)

## Debit Spreads

### Bull Call Spread

**Structure:**
- Buy ATM/slightly OTM call
- Sell further OTM call
- Net debit
- Bullish trade

**Example:**
```markdown
## Bull Call Spread on NVDA

**Underlying:** NVDA at $500

**Structure:**
- Buy $500 call @ $15.00
- Sell $520 call @ $8.00
- Net debit: $7.00 ($700 per spread)

**Risk/Reward:**
- Max profit: $1,300 (if NVDA above $520)
- Max loss: $700 (debit paid)
- Breakeven: $507
- Risk/Reward: 1.86:1

**Thesis:** NVDA rallies to $520+ (20 points up)

**Management:**
- Take profit at 50-75% of max
- Cut loss if stock reverses hard
- Exit before expiration
```

### Bear Put Spread

**Structure:**
- Buy ATM/slightly OTM put
- Sell further OTM put
- Net debit
- Bearish trade

**Use:** Strong bearish conviction (cheaper than buying puts outright)

## Calendar Spreads

### What It Is

**Structure:**
- Sell near-term option (30 DTE)
- Buy longer-term option (60-90 DTE)
- Same strike (ATM typically)
- Net debit

**Goal:** Front month decays faster than back month

**Example:**
```markdown
## Calendar Spread on SPY

**Underlying:** SPY at $420

**Structure:**
- Sell SPY $420 call, 30 DTE @ $5.00
- Buy SPY $420 call, 60 DTE @ $7.00
- Net debit: $2.00 ($200 per calendar)

**Profit scenario:**
- Front month expires worthless
- Back month retains value
- Stock stays near $420

**Management:**
- Front month expires: collect profit
- Sell another front month (turn into diagonal)
- Close both if stock moves away
```

**Best for:**
- Neutral outlook
- High IV (sell expensive front month)
- Theta decay capture

## Advanced Position Sizing

### Risk-Based Sizing

**Rule:** Risk X% of account per trade

**Example:**
```
Account: $50,000
Risk per trade: 2% = $1,000

Iron Condor with $300 max loss:
Can put on 3 ICs ($300 × 3 = $900 risk)

Credit spread with $500 max loss:
Can put on 2 spreads ($500 × 2 = $1,000 risk)
```

### Portfolio Heat

**Track total risk across all positions:**
```markdown
## Current Portfolio Risk

Position 1: SPY IC - Max risk $400
Position 2: QQQ BWB - Max risk $300
Position 3: AAPL Call Spread - Max risk $500
Position 4: MSFT Put Spread - Max risk $600

Total risk: $1,800
Account: $50,000
Portfolio heat: 3.6%

Rule: Keep total risk <10% of account
```

## Strategy Selection Framework

**Decision tree:**
```
Market outlook?
│
├── Neutral → Iron Condor or Butterfly
│   └── High IV? → Iron Condor
│   └── Low IV? → Skip or Butterfly
│
├── Bullish → Bull Put Spread or Bull Call Spread
│   └── High confidence? → Debit spread (call)
│   └── Medium confidence? → Credit spread (put)
│
├── Bearish → Bear Call Spread or Bear Put Spread
│   └── High confidence? → Debit spread (put)
│   └── Medium confidence? → Credit spread (call)
│
└── Sideways with bias → Broken Wing Butterfly
    └── Slightly bullish? → Bearish BWB (profit if pins or drops)
    └── Slightly bearish? → Bullish BWB (profit if pins or rises)
```

## Risk Management

### Position Management Rules

**1. Entry checklist:**
- [ ] IV rank >30th percentile (for credit strategies)
- [ ] Liquid options (volume >100, spread <5%)
- [ ] Risk appropriate for account (2-5% per position)
- [ ] Clear thesis (why this trade?)
- [ ] No earnings in next 2 weeks
- [ ] Position doesn't over-concentrate portfolio

**2. During trade:**
- [ ] Monitor daily (set alerts)
- [ ] Check at 21 DTE (manage or close)
- [ ] Take profit at 50% (don't be greedy)
- [ ] Cut loss if thesis breaks
- [ ] Adjust if needed (roll, close side, etc.)

**3. Exit rules:**
- Close at 50% max profit (standard)
- Close at 21 DTE if still profitable
- Cut loss at 2x credit collected (for credit strategies)
- Exit if thesis invalidated

### Common Adjustments

**For Iron Condors:**

**1. Roll tested side**
```
Call side tested (stock rallied):
- Close call spread (take loss)
- Sell new call spread higher (collect credit)
- Net: Extended duration, moved strikes up
```

**2. Close untested side**
```
Call side tested, put side safe:
- Close put spread (small profit)
- Let call spread resolve
- Reduces risk, takes some profit
```

**For Butterflies/BWBs:**

**1. Roll center**
```
Stock moved away from center:
- Close current butterfly
- Open new butterfly at new center
- Follow the stock
```

**2. Widen wings**
```
Add protection if needed:
- Buy additional wing for more defense
- Costs money but reduces max loss
```

## Performance Tracking

### Trade Log Template
```markdown
## [Strategy] on [Ticker] - [Date]

**Setup:**
- Underlying: [Ticker] at $X
- Strategy: [IC, BWB, Spread, etc.]
- Structure: [Specific strikes and expirations]
- Credit/Debit: $X
- Max profit: $X
- Max loss: $X
- Breakevens: $X and $X

**Thesis:**
[Why this trade? What's the expectation?]

**Entry date:** [Date]
**DTE at entry:** X days
**Risk:** $X (X% of account)

**Management plan:**
- Take profit at: 50% ($X)
- Cut loss at: $X
- Adjust if: [Conditions]

**Result:**
- Exit date: [Date]
- Exit P/L: $X (+/- X%)
- Exit reason: [50% profit, 21 DTE, thesis broken, etc.]
- Held for: X days

**Lessons:**
[What worked? What didn't? What to do differently?]
```

### Key Metrics

**Track per strategy:**
```
Iron Condors:
- Win rate: X%
- Average return: X%
- Average hold time: X days
- Best trade: $X
- Worst trade: -$X

Butterflies:
- Win rate: X%
- Average return: X%
...etc
```

**Overall portfolio:**
```
Total trades: X
Winners: X (X%)
Losers: X (X%)
Average return per trade: X%
Total P/L: $X
Account return: X%
```

## Integration with Other Skills

### With Equity Research
**Trade advanced strategies on researched stocks:**
- Iron condors on quality names
- Butterflies on stable companies
- Directional spreads after deep dive

### With Portfolio Manager
**Advanced strategies as portfolio component:**
- Allocate X% of portfolio to options
- Track separately from buy-and-hold
- Include in risk management

### With Options Wheel
**Complementary strategies:**
- Wheel for income + shares
- Advanced for defined risk + higher returns
- Use both depending on market

### With Tax Optimizer
**Tax considerations:**
- All gains/losses short-term (held <1 year typically)
- Frequent trading = more tax events
- Consider in tax-advantaged accounts

## Common Mistakes

❌ **Avoid:**
- Trading low IV (not enough premium for credit strategies)
- Undefined risk (these are all defined-risk, keep it that way)
- Over-leveraging (small account, too many positions)
- Letting winners become losers (take 50% profit!)
- Holding to expiration (pin risk, gamma risk)
- Trading earnings (volatility spike, unpredictable)
- Ignoring adjustments (manage trades, don't set and forget)

✅ **Do:**
- Trade high IV rank (>50th percentile for ICs)
- Keep risk per trade small (2-5%)
- Take profit at 50% (proven to improve returns)
- Close/adjust at 21 DTE
- Avoid earnings
- Track everything (learn from data)
- Stay disciplined (rules > emotions)

## Tools

**Options platforms:**
- ThinkorSwim (best analysis)
- Tastyworks (designed for these strategies)
- Interactive Brokers (low commissions)

**Analysis:**
- OptionStrat (visualize any strategy)
- OptionsProfitCalculator.com
- TradingView (charts)

**IV Rank:**
- Barchart
- MarketChameleon
- TastyTrade platform

## Deliverables

For each advanced strategy trade:
1. **Trade plan:** Structure, risk/reward, thesis
2. **Entry execution:** Fills, actual credit/debit
3. **Management log:** Daily/weekly checks
4. **Exit analysis:** Why closed, P/L, lessons
5. **Performance tracking:** Running statistics

## Next Steps

To use advanced strategies:
1. [ ] Choose strategy based on market outlook
2. [ ] Paper trade first (3-5 trades minimum)
3. [ ] Start small (1-2 contracts)
4. [ ] Track meticulously
5. [ ] Scale up as profitable

What strategy should we start with?