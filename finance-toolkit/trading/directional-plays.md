---
name: directional-plays
description: Directional options strategies for bullish, bearish, and volatility plays
category: Options Trading
tags: [options, directional, calls, puts, spreads, volatility, speculation]
version: 1.0.0
---

# Directional Plays

Expert in directional options trading strategies. Help execute bullish, bearish, and volatility plays using long options, spreads, and advanced multi-leg strategies when you have a strong conviction about market direction.

## Core Principles

**Directional trading is speculation, not income**
- Different mindset than wheel/theta strategies
- Higher risk, higher potential reward
- Win rate typically 30-50% (vs 70-80% for theta)
- Home runs offset strikeouts

**Conviction required**
- Don't trade direction without edge
- Technical setup + catalyst + timing
- If unsure, don't trade

**Position sizing is critical**
- Each trade: 1-5% of portfolio max
- Total directional exposure: 10-20% max
- Keep majority in theta/investment strategies

**Goal:** Asymmetric risk/reward on high-conviction setups

---

## When to Trade Directionally

### Good reasons to make a directional play:

**Strong technical setup:**
```
Examples:
- Breakout from consolidation
- Clear support/resistance levels
- Trend continuation pattern
- Volume confirmation

Not good enough alone, but necessary foundation
```

**Catalyst identified:**
```
Examples:
- Earnings beat anticipated (with edge)
- FDA approval coming
- Product launch
- Regulatory change
- Macro event

Timing is everything
Market often prices in obvious catalysts
Need non-consensus view
```

**Risk/reward favorable:**
```
Minimum 3:1 reward to risk
Preferably 5:1 or better

Example:
Risk: $500 on long call
Potential: $2,500+ if right
Ratio: 5:1

Worth it if probability > 20%
```

**Clear invalidation point:**
```
Know when you're wrong

Example: Long call on breakout
Stop loss: If breaks back below support
Clear, objective, no hoping
```

### Bad reasons to trade directionally:

```
✗ Bored, want action
✗ FOMO from others' gains
✗ "Feels like" it should move
✗ Trying to make back losses
✗ News already priced in
✗ No clear thesis
✗ Random TA pattern without context
✗ Position too large
```

---

## Bullish Strategies

### Long Call

**The simplest directional play**

**Setup:**
```
- Believe stock will move up significantly
- Want unlimited upside potential
- Accept 100% loss risk
- Short time horizon (30-90 days typical)
```

**Mechanics:**
```
Buy 1 call option

Example: Stock at $100
Buy $105 call, 45 DTE
Cost: $300

Breakeven: $105 + $3 = $108
Max loss: $300 (100%)
Max gain: Unlimited
```

**When to use:**
```
✓ Strong bullish conviction
✓ Expected move > 10-15%
✓ Clear catalyst within timeframe
✓ High implied volatility not a concern (or you expect it to rise)
```

**Strike selection:**
```
ATM (At The Money): Most sensitive to price movement
- Delta ~0.50
- Most common for directional trades
- Balance of leverage and probability

ITM (In The Money): More expensive, higher probability
- Delta 0.60-0.80
- Less leverage, more capital required
- Safer but lower ROI

OTM (Out of The Money): Cheaper, lower probability
- Delta 0.20-0.40
- Lottery ticket territory
- High leverage, high risk
```

**Example trade:**
```
Setup: AAPL at $175, strong breakout pattern
Catalyst: Product launch in 30 days
Thesis: Move to $185+ likely

Trade: Buy $180 call, 45 DTE
Cost: $400
Delta: 0.40

Scenarios:

Stock to $190 (up $15):
Call value: ~$1,200
Profit: $800 (200% return)

Stock to $180 (up $5):
Call value: ~$600
Profit: $200 (50% return)

Stock to $170 (down $5):
Call value: ~$50
Loss: $350 (87.5% loss)

Stock unchanged:
Call value: ~$100 (time decay)
Loss: $300 (75% loss)
```

**Management:**
```
Take profit: 50-100% gain (don't get greedy)
Stop loss: -50% or technical invalidation (whichever first)
Time decay: Exit if 2 weeks left and not ITM
Never hold to expiration unless deep ITM
```

---

### Bull Call Spread

**Defined risk version of long call**

**Setup:**
```
- Bullish but want to reduce cost
- Accept capped upside
- Lower breakeven than naked long call
- More conservative directional play
```

**Mechanics:**
```
Buy lower strike call
Sell higher strike call (same expiration)

Example: Stock at $100
Buy $105 call: -$400
Sell $110 call: +$150
Net cost: $250

Breakeven: $105 + $2.50 = $107.50
Max loss: $250
Max gain: $250 (at $110+)
```

**Math:**
```
Max gain = (Width of strikes) - (Net debit)
Max gain = ($110 - $105) - $2.50 = $2.50

ROI potential: $250 gain / $250 risk = 100%
Probability of profit: Higher than long call (lower breakeven)
```

**When to use:**
```
✓ Moderately bullish (not expecting huge move)
✓ High IV (short call reduces cost)
✓ Clear target price (sell strike at target)
✓ Want defined risk
```

**Example trade:**
```
Setup: TSLA at $250, expect rally to $270
IV: High (60%)
Timeframe: 60 days

Trade: 
Buy $260 call: -$800
Sell $270 call: +$400
Net: $400

At expiration:

Stock at $280:
Both calls ITM
Spread worth: $10 width = $1,000
Profit: $600 (150%)

Stock at $265:
Long call worth ~$500
Short call worthless
Profit: $100 (25%)

Stock at $255:
Spread worth ~$200
Loss: $200 (50%)

Stock at $245:
Both worthless
Loss: $400 (100%)
```

**Spread width selection:**
```
Narrow spreads ($5 wide):
- Less capital required
- Lower max gain
- Higher breakeven probability

Wide spreads ($10-20 wide):
- More capital required  
- Higher max gain
- Acts more like long call

Sweet spot: $5-10 wide for most trades
```

---

### Cash-Secured Put (Bullish version)

**Covered in wheel strategy, but directional application:**

**Setup:**
```
- Bullish, want to own stock
- Stock pulled back to support
- Getting paid to enter position
```

**Mechanics:**
```
Sell put at desired entry price
Secure with cash

Example: Stock at $105, want to own at $100
Sell $100 put, 30 DTE
Collect: $300

Outcomes:
Stock above $100: Keep $300, try again
Stock below $100: Buy 100 shares at $100, net cost $97
```

**Directional edge:**
```
Unlike wheel strategy (mechanical), directional CSP is targeted:
- Specific entry price (not just "at current price")
- Technical level (support, moving average)
- Short duration (30-45 DTE max)
- Don't roll aggressively (accept assignment)
```

---

## Bearish Strategies

### Long Put

**Inverse of long call**

**Setup:**
```
- Believe stock will move down significantly
- Want unlimited downside profit potential
- Accept 100% loss risk
- Portfolio hedge or speculation
```

**Mechanics:**
```
Buy 1 put option

Example: Stock at $100
Buy $95 put, 45 DTE
Cost: $300

Breakeven: $95 - $3 = $92
Max loss: $300 (100%)
Max gain: $95 per share ($9,200 if stock goes to zero)
```

**When to use:**
```
✓ Strong bearish conviction
✓ Expected move down > 10-15%
✓ Bear market environment
✓ Protect long portfolio (hedge)
```

**Hedging application:**
```
Portfolio: $100k in stocks
Risk: Market crash

Protection: Buy $SPY puts
Buy 10x $450 puts (SPY at $470), 60 DTE
Cost: $3,000 (3% of portfolio)

If SPY drops 20% to $376:
Puts worth: ~$70 each = $70,000
Portfolio loss: ~$20,000
Net: $50,000 gain

Insurance cost: $3k (worth it for 20% crash protection)
```

**Example trade:**
```
Setup: NVDA at $500, parabolic run, RSI >80
Catalyst: None, pure momentum
Thesis: Pullback to $450 likely

Trade: Buy $480 put, 45 DTE
Cost: $600
Delta: -0.35

Scenarios:

Stock to $450 (down $50):
Put value: ~$3,000
Profit: $2,400 (400% return)

Stock to $480 (down $20):
Put value: ~$1,200
Profit: $600 (100% return)

Stock to $520 (up $20):
Put value: ~$50
Loss: $550 (92% loss)
```

---

### Bear Put Spread

**Defined risk version of long put**

**Setup:**
```
- Bearish but want to reduce cost
- Accept capped profit
- Lower breakeven than naked long put
```

**Mechanics:**
```
Buy higher strike put
Sell lower strike put (same expiration)

Example: Stock at $100
Buy $95 put: -$400
Sell $90 put: +$150
Net cost: $250

Breakeven: $95 - $2.50 = $92.50
Max loss: $250
Max gain: $250 (at $90 or below)
```

**When to use:**
```
✓ Moderately bearish
✓ High IV (short put reduces cost)
✓ Clear target price (sell strike at target)
✓ Want defined risk
```

**Example trade:**
```
Setup: SPY at $470, expect pullback to $455
IV: Elevated (25%)
Timeframe: 45 days

Trade:
Buy $465 put: -$600
Sell $455 put: +$250
Net: $350

At expiration:

Stock at $445:
Both puts ITM
Spread worth: $10 width = $1,000
Profit: $650 (186%)

Stock at $460:
Long put worth ~$500
Short put worthless  
Profit: $150 (43%)

Stock at $465:
Spread worth ~$150
Loss: $200 (57%)

Stock at $475:
Both worthless
Loss: $350 (100%)
```

---

### Bear Call Spread

**Credit spread, bearish assumption**

**Setup:**
```
- Mildly bearish or neutral
- Want to collect credit
- Stock resistance level
- Defined risk short strategy
```

**Mechanics:**
```
Sell lower strike call
Buy higher strike call (same expiration)

Example: Stock at $100
Sell $105 call: +$300
Buy $110 call: -$100
Net credit: $200

Max profit: $200 (if stock below $105)
Max loss: $300 (if stock above $110)
Breakeven: $105 + $2 = $107
```

**When to use:**
```
✓ Bearish or neutral
✓ Stock at resistance
✓ High IV (maximize credit)
✓ Probability play (not huge move expected)
```

**Risk management:**
```
Position size: Max loss should be 1-2% of portfolio
Stop loss: If stock breaks above short strike, consider closing
Don't be a hero: Close at 50% max loss, don't wait for max loss
```

---

## Volatility Strategies

### Long Straddle

**Bet on big move, either direction**

**Setup:**
```
- Expect large move but unsure of direction
- Catalyst coming (earnings, FDA, etc.)
- Current IV lower than expected move
```

**Mechanics:**
```
Buy ATM call
Buy ATM put (same strike, same expiration)

Example: Stock at $100
Buy $100 call: -$500
Buy $100 put: -$450
Total cost: $950

Breakeven: $100 ± $9.50 = $90.50 or $109.50
Max loss: $950 (if stock unchanged)
Max gain: Unlimited (large move either way)
```

**When to use:**
```
✓ Major catalyst (earnings, trial results, etc.)
✓ IV not yet elevated (buy before run-up)
✓ Expected move > breakeven range
✓ Don't know direction but expect volatility
```

**Earnings example:**
```
Setup: TSLA at $250, earnings tomorrow
Historical earnings move: ±12%
IV: 80% (implies ~8% move)
Thesis: Bigger move than priced in

Trade:
Buy $250 call: -$1,200
Buy $250 put: -$1,100
Total: $2,300

Breakeven: $250 ± $23 = $227 or $273 (9.2% move)

Post-earnings:

Stock to $280 (up 12%):
Call worth: ~$3,000
Put worth: ~$50
Profit: $750 (33%)

Stock to $220 (down 12%):
Put worth: ~$3,000
Call worth: ~$50
Profit: $750 (33%)

Stock to $255 (up 2%):
Call worth: ~$800
Put worth: ~$200
Loss: $1,300 (57%)

Risk: IV crush - even if stock moves, both options lose value if IV drops
```

**IV crush problem:**
```
Before earnings: IV = 80%
After earnings: IV drops to 40% (typical)

Even with 5% stock move:
- Options lose 50% value from IV drop
- May still lose money overall

Solution: 
- Buy straddle well before earnings (1-2 weeks)
- Close before earnings if IV spike sufficient
- OR commit to holding through and need bigger move
```

---

### Long Strangle

**Cheaper version of straddle**

**Setup:**
```
- Expect large move but unsure of direction
- Want to reduce cost vs. straddle
- Accept wider breakeven range
```

**Mechanics:**
```
Buy OTM call
Buy OTM put (same expiration)

Example: Stock at $100
Buy $105 call: -$300
Buy $95 put: -$250
Total cost: $550

Breakeven: $105 + $5.50 = $110.50 or $95 - $5.50 = $89.50
Max loss: $550
Max gain: Unlimited
```

**Straddle vs. Strangle:**
```
Straddle (ATM):
- Cost: Higher ($950)
- Breakevens: Narrower (±9.5%)
- Better if: Moderate move expected

Strangle (OTM):
- Cost: Lower ($550)
- Breakevens: Wider (±10.5-11%)
- Better if: Large move expected
```

---

### Short Straddle/Strangle

**Opposite: Bet on no movement**

**Setup:**
```
- Expect stock to stay in range
- Collect premium from high IV
- Undefined risk (dangerous)
```

**Mechanics:**
```
Sell ATM call
Sell ATM put

Example: Stock at $100
Sell $100 call: +$500
Sell $100 put: +$450
Total credit: $950

Max profit: $950 (if stock exactly at $100)
Max loss: Unlimited
Breakeven: $90.50 or $109.50
```

**Why dangerous:**
```
Black swan risk:
Stock gaps 20%+ overnight
Loss: Potentially $10,000+ on $950 credit
Risk/reward: Terrible

Only for advanced traders with:
- Small position sizes
- Tight stop losses
- Hedging strategies
- Strong risk management
```

**Better alternative: Iron Condor (defined risk version)**

---

## Advanced Multi-Leg Strategies

### Ratio Spread

**Bullish with capped profit, risky above**

**Setup:**
```
- Bullish to a point
- Expect move to specific level, not beyond
- Want to reduce cost or create credit
```

**Mechanics:**
```
Buy 1 ATM call
Sell 2 OTM calls

Example: Stock at $100
Buy $100 call: -$500
Sell 2x $110 calls: +$300
Net: $200 debit

Max profit: At $110 (long call ITM $10, short calls worthless)
Profit: $1,000 - $200 = $800
Max loss: Unlimited (if stock above $120)
```

**Risk profile:**
```
Below $100: Lose $200 (max loss on downside)
At $110: Max profit $800
Above $120: Unlimited loss (2 short calls outpace 1 long)

Danger zone: Stock moves way beyond expectation
```

**When to use:**
```
✓ High conviction on exact price target
✓ Don't expect move beyond target
✓ Very specific scenario

Usually better to just do bull call spread (defined risk)
```

---

### Calendar Spread (Time Spread)

**Bet on time decay difference**

**Setup:**
```
- Stock stays at or near current price
- Profit from near-term theta faster than long-term
- Directionally neutral or slightly directional
```

**Mechanics:**
```
Sell near-term option
Buy longer-term option (same strike)

Example: Stock at $100
Sell $100 call, 30 DTE: +$300
Buy $100 call, 90 DTE: -$500
Net: $200 debit

At front-month expiration:
- If stock at $100: Short call expires worthless, long call worth ~$300
- Profit: $100
- Can sell another 30 DTE call against long call
```

**When to use:**
```
✓ Low volatility environment
✓ Range-bound stock
✓ Want to reduce long option cost
✓ Theta strategy with directional component
```

**Risks:**
```
- Large move either direction can hurt
- Needs to manage after front month expires
- Vega risk (if IV changes)
- More complex than simple directional plays
```

---

### Diagonal Spread

**Calendar spread + different strikes**

**Setup:**
```
- Slightly bullish or bearish
- Want theta advantage plus directional bias
```

**Mechanics:**
```
Sell near-term OTM option
Buy longer-term ITM or ATM option (different strike)

Bullish example: Stock at $100
Sell $105 call, 30 DTE: +$200
Buy $100 call, 90 DTE: -$500
Net: $300 debit

If stock at $105 at front expiration:
- Short call expires worthless
- Long call worth ~$600
- Profit: $300
- Can sell another 30 DTE call
```

---

## Position Sizing & Risk Management

### Position sizing rules:

**Single trade:**
```
Aggressive: 5% of portfolio max
Moderate: 2-3% of portfolio
Conservative: 1% of portfolio

$50k portfolio:
- Max single trade: $2,500 (5%)
- Typical trade: $1,000-1,500 (2-3%)
- Conservative: $500 (1%)

Never put more than 5% in single directional trade
These are speculation, not investments
```

**Total directional exposure:**
```
Max: 10-20% of portfolio in all directional trades combined

$50k portfolio:
- Max directional total: $10k (20%)
- All other positions: Theta strategies, stocks, etc.

Keep majority in income/investment strategies
Directional is enhancement, not core
```

### Stop losses:

**Price-based:**
```
Long calls/puts:
- Stop at -50% loss (half gone = time to exit)
- OR if technical setup invalidated
- Whichever comes first

Spreads:
- Stop at -50% of max loss
- $250 max loss spread: Stop at -$125
```

**Time-based:**
```
Don't hold options to expiration unless deep ITM

Long options:
- Exit if 2 weeks left and not ITM
- Theta accelerates drastically
- Unlikely to recover

Exception: Let winners run if still ITM with 2 weeks left
```

**Technical invalidation:**
```
Trade based on breakout above $50 resistance:
- Stop loss: If price breaks back below $50
- Doesn't matter if option is down 20% or 40%
- Setup failed = exit

Be objective, not hopeful
```

### Profit taking:

**Ladder out:**
```
Don't sell all at once

Example: 3 long calls
- Sell 1 at 50% profit (take off 1/3)
- Sell 1 at 100% profit (take off another 1/3)  
- Let 1 run (playing with house money)

Captures profit, keeps upside
```

**Trailing stop:**
```
Once at 50%+ profit:

Move stop to breakeven (can't lose)
Then trail:
- If hits 100%: Move stop to +50%
- If hits 150%: Move stop to +100%

Locks in gains while allowing upside
```

---

## Example Trade Setups

### Setup 1: Breakout long call

```
Technical: Stock consolidating at $100 for 2 months, attempting breakout
Volume: Increasing on up days
Catalyst: None specific (technical play)
Timeframe: 45 days

Trade: Buy $105 call, 45 DTE
Cost: $350
Delta: 0.40

Entry: On break above $102 with volume
Stop: If breaks back below $100
Target: $115 (15% move)

Risk: $350
Reward: ~$1,000+ (3:1 R/R)

Management:
- Sell half at 50% profit ($525)
- Let rest run with trailing stop
```

### Setup 2: Earnings bull call spread

```
Fundamental: Expect earnings beat
Technical: Stock at support ($95)
IV: Elevated at 70%
Timeframe: Earnings in 30 days

Trade: Bull call spread
Buy $100 call: -$400
Sell $110 call: +$200
Net: $200

Entry: 1 week before earnings
Exit: Day after earnings (don't hold through IV crush more than necessary)

Risk: $200
Reward: $800 (4:1 R/R)

Why spread vs long call:
- High IV makes long call expensive
- Sell call to reduce cost
- Defined risk appropriate for binary event
```

### Setup 3: Put hedge

```
Portfolio: $100k, 100% long stocks
Market: Extended, potential correction
Goal: Protection, not speculation

Trade: Buy SPY puts
Buy 5x $460 puts (SPY at $480), 90 DTE
Cost: $2,500 (2.5% of portfolio)
Delta: -0.25 per contract = -125 deltas total

If market drops 10%:
Portfolio loses: ~$10k
Puts gain: ~$10k
Net: Protected

If market rises 10%:
Portfolio gains: ~$10k
Puts lose: $2,500 (cost)
Net: $7,500 gain (insurance cost)

Annual insurance cost: ~$10k (10% drag)
Worth it? Depends on risk tolerance and market conditions
```

### Setup 4: Volatility play (strangle)

```
Event: FDA decision in 30 days
Stock: Biotech at $50
Historical moves: ±25% on FDA news
IV: 100% (implies 15% move - too low)

Trade: Long strangle
Buy $55 call: -$400
Buy $45 put: -$350
Total: $750

Breakeven: $55 + $7.50 = $62.50 (+25%)
         : $45 - $7.50 = $37.50 (-25%)

If approved, stock to $65:
Call worth: ~$1,000
Put worth: ~$0
Profit: $250 (33%)

If denied, stock to $35:
Put worth: ~$1,000
Call worth: ~$0
Profit: $250 (33%)

If no decision or stock at $50:
Loss: $750 (100%)

Risk/reward makes sense if probability of >25% move is >40%
```

---

## Common Mistakes

### Mistake 1: Trading directionally without edge

```
Problem: "Feels like AAPL will go up"
No analysis, no setup, just gambling

Fix:
- Require technical setup
- Identify catalyst
- Calculate risk/reward
- No trade if no edge
```

### Mistake 2: Position too large

```
Problem: $10k portfolio, buy $5k in calls
One wrong trade = 50% loss

Fix:
- Max 5% per trade
- Max 20% total directional
- Keep majority in safer strategies
```

### Mistake 3: No stop loss

```
Problem: Down 80%, "waiting for comeback"
Hope is not a strategy

Fix:
- Set stop at entry (price or time)
- Stick to it
- -50% max loss on long options
```

### Mistake 4: Holding to expiration

```
Problem: "Maybe it'll recover in last 3 days"
Theta is -$30/day, stock needs miracle

Fix:
- Exit 2 weeks before expiration if not ITM
- Don't fight theta acceleration
- Exception: Already deep ITM
```

### Mistake 5: Buying expensive options

```
Problem: IV at 150%, buy calls anyway
Even if stock moves right, you lose (IV crush)

Fix:
- Check IV percentile (avoid >80%)
- Consider spreads to reduce vega risk
- Or skip the trade
```

### Mistake 6: Revenge trading

```
Problem: Lost $1k, immediately open $2k position to "make it back"
Emotional trading = disaster

Fix:
- Walk away after loss
- Review trade objectively later
- Don't increase size after loss
```

---

## Integration with Other Finance Areas

### With Portfolio Manager
**Directional plays are speculation, not core holdings:**
- Track separately from long-term investments
- Don't confuse speculation with investing
- Limit to small percentage of total portfolio

### With Budget Manager
**Directional trading capital must be accounted for:**
- Set monthly/annual speculation budget
- Losses come from this budget, not emergency fund
- Wins are bonus, not expected income

### With Options Wheel
**Different strategies, different purposes:**
```
Wheel: Income generation, high win rate
Directional: Speculation, lower win rate but big wins

Allocation example:
- 70% portfolio: Long-term stocks
- 20%: Wheel strategies (income)
- 10%: Directional plays (speculation)

Don't confuse the two
Different risk profiles, different mindsets
```

---

## Tools & Analysis

**Technical analysis:**
- TradingView (charts, indicators)
- thinkorswim (analysis tools)
- Technical patterns: Support/resistance, breakouts, trends

**Options analysis:**
- Options profit calculator
- IV rank/percentile (avoid high IV)
- Expected move calculator

**Trade journaling:**
- Every trade: Setup, thesis, result
- Win/loss tracking
- Review monthly: What's working, what's not

---

## Deliverables

After directional play analysis:

1. **Trade Setup:** Technical levels, catalyst, thesis
2. **Position Structure:** Strikes, expiration, cost
3. **Risk Parameters:** Max loss, stop loss, position size
4. **Profit Targets:** Exit plan at various profit levels
5. **Invalidation Point:** When setup is wrong, exit

---

## Red Flags

**Don't trade if:**
```
☐ No clear thesis ("just feels like it'll move")
☐ Position size >5% of portfolio
☐ Can't afford to lose the capital
☐ Chasing a move already happened
☐ Revenge trading (trying to recover losses)
☐ IV extremely high (>80th percentile)
☐ No technical setup
☐ No catalyst identified
☐ Risk/reward < 2:1
☐ No stop loss plan
```

---

## Final Thoughts

**Directional trading is hard**
- Win rate: 30-50% typically
- Requires discipline, analysis, and risk management
- Most traders lose money doing this

**Home runs make it worth it**
- One 10-bagger can offset 10 small losses
- Asymmetric risk/reward
- Small % of portfolio, large potential impact

**Stay disciplined:**
- Position sizing rules: Non-negotiable
- Stop losses: Always set, always honor
- Don't overtrade: Quality setups only
- Journal everything: Learn from wins AND losses

**Directional is speculation, not income**
- Don't rely on it for living expenses
- Supplement to core investment strategy
- Keep expectations realistic

Let's identify high-probability setups.