---
created: 
basis: TBD
tags:
---

# Daily Trade Report Criteria

Update this file weekly — or immediately when macro conditions shift significantly.
The report reads this file before running, then re-evaluates every layer against
current live data. This file sets the framework. Live data determines the output.
If current data contradicts any assumption written here, current data wins — and the
report must state the divergence explicitly.

---

## Advisor Directive

This report runs in ruthless advisor mode. No sugarcoating. No burying risk.
Every setup is stress-tested through the full curriculum stack before it appears.
Incomplete setups are excluded, not softened. Tail risks are stated plainly.
If fewer than 4 securities pass the full stack, fewer than 4 are recommended.
A short list of real setups is better than a full list of marginal ones.

---

## Step 0 — Full Environment Re-Assessment (Run Before Anything Else)

Before a single security is screened, answer every question below from current data.
These answers determine which sections of the framework apply and which divergence
rules activate. Do not skip this step.

### Broad Market Stage (Weinstein)
- Where is the S&P 500 relative to its 30-week MA? Above (Stage 1/2) or below (Stage 3/4)?
- Is the 30-week MA trending up, flat, or turning down?
- How many of the 11 S&P sectors are currently in Stage 2? (Majority = bull environment. Minority = distribution or bear.)

### Market Breadth (Murphy)
- Is the advance/decline line trending up or down over the last 10 days?
- New 52-week highs vs. new 52-week lows: which side has the majority?
- If the index is rising but breadth is deteriorating — narrow rally. Flag it. Reduce recommendations to 2 and require VCP base breakouts only (no momentum continuation entries).

### Intermarket Relationships (Murphy + Dalio)
- **US Dollar (DXY):** Strengthening or weakening vs. prior week?
  - Dollar strengthening = headwind for commodities, EM names (YPF, etc.), and materials
  - Dollar weakening = tailwind for energy, gold, EM equities
- **10-Year Treasury Yield:** Rising or falling?
  - Rising yields = tightening financial conditions = headwind for growth, small-cap, high-multiple names
  - Falling yields = easing conditions = tailwind for rate-sensitive sectors (utilities, REITs)
- **Oil (WTI/Brent):** Direction and magnitude of move vs. prior 5 days?
  - Oil up >5% in a week = energy sector tailwind, consumer discretionary headwind, inflation risk
  - Oil down >5% in a week = re-evaluate all energy positions; if in an oil-driven trade, tighten stops immediately
- **Credit spreads:** Widening or tightening?
  - Widening spreads = institutional risk-off signal; reduce new position sizing, avoid small-cap and high-yield names
  - Tightening spreads = risk-on; standard position sizing applies

### RSI Market Regime (Brown)
Identify the current regime before reading any oscillator on any chart.
- **Bull regime:** RSI oscillates 40–90. "Oversold" = ~40–50. "Overbought" = ~80–90.
- **Bear regime:** RSI oscillates 10–60. "Oversold" = ~10–20. "Overbought" = ~50–60.
- Determine current regime from the weekly S&P 500 RSI. Apply the correct thresholds to every individual chart. Fixed 70/30 thresholds are only valid in neutral markets — using them in a trending regime produces systematically wrong reads.

### Macro Cycle Position (Marks + Dalio)
- Where is sentiment: fear dominant, neutral, or greed dominant? (VIX level, news tone, analyst commentary)
- Are credit conditions tightening or loosening? (Fed language, credit spread direction, lending standards)
- Where are we in the debt cycle? Early expansion, mid-cycle, late-cycle, or deleveraging?
- Is this an inflationary or deflationary environment? (Determines which assets outperform — commodities/energy in inflation; bonds/defensive in deflation)
- Apply Marks second-level thinking: Is the current consensus thesis already priced into the sector? If energy is up 39% in 3 weeks, the easy money may already be made. Ask where the market is wrong, not where it is right.

---

## Divergence Rules — When to Override Standard Categories

These are the conditions under which the report must deviate from the default sector focus,
criteria, or position sizing. Re-evaluate these triggers on every run.

### Divergence 1 — Broad Market in Stage 3 or 4
**Trigger:** S&P 500 below its 30-week MA and MA turning down.
**Override:**
- Suspend all long recommendations in cyclical sectors (energy, materials, industrials, financials)
- Defensive sectors only: utilities, consumer staples, healthcare — and only if they are individually in Stage 2
- Reduce max positions from 4 to 2
- Consider inverse ETFs (SH, SDS, SPXU) or sector short ETFs as part of the recommendation set
- Position size reduced to 0.5% risk per trade until Stage 2 re-establishes on the weekly chart

### Divergence 2 — Narrow Market Rally (Index Up, Breadth Deteriorating)
**Trigger:** S&P 500 rising but A/D line declining, or fewer than 40% of S&P components above their 50-day MA.
**Override:**
- Do not treat index strength as a green light for new longs
- Only recommend securities in the specific sectors driving the narrow rally
- Require VCP base breakout confirmation — no momentum continuation entries
- Flag the breadth divergence prominently at the top of the report

### Divergence 3 — Oil Spike Reversal Signal
**Trigger:** Oil drops more than 5% in a single session, OR a geopolitical de-escalation event is reported (ceasefire, negotiations, Strait of Hormuz reopening).
**Override:**
- Suspend all energy sector long recommendations until oil re-establishes above its prior support level
- Existing energy positions: move stops to breakeven or tighten to prior swing low
- Consider energy consumer beneficiaries (airlines, trucking, consumer discretionary) as replacement candidates if their technicals confirm
- YPF and other EM oil names get suspended first — highest currency/political risk

### Divergence 4 — Dollar Strengthening Sharply (>2% in One Week)
**Trigger:** DXY rising more than 2% in a 5-day period.
**Override:**
- Remove or flag all emerging market names (YPF, etc.) — dollar strength compresses EM earnings and triggers capital outflows
- Commodity-denominated names (MEOH, gold miners, base metals) face dollar headwind — require tighter confirmation before recommending
- Domestically-focused US names with no significant export revenue become relatively more attractive

### Divergence 5 — Credit Spreads Widening
**Trigger:** Investment grade or high-yield spreads widen more than 25 bps in a week.
**Override:**
- Avoid small-cap and mid-cap names regardless of technicals — institutional liquidity is withdrawing
- Stick to large-cap, highly liquid names only
- Reduce all position sizes by 50%
- This is an early warning of institutional risk-off — do not fight it with individual stock picks

### Divergence 6 — VIX Above 30
**Trigger:** VIX (volatility index) closes above 30.
**Override:**
- Standard entry rules are suspended. High-volatility environments produce excessive whipsaws at normal stop distances.
- Widen stops to the next significant technical level (not the standard 5–8%)
- Reduce position size to compensate: if stop widens from 5% to 10%, cut shares in half to keep dollar risk at 1%
- Prioritize ETFs over individual stocks — diversified exposure reduces single-name gap risk
- Consider waiting for VIX to begin contracting before entering new positions

### Divergence 7 — Parabolic Sector Move (>25% in 30 Days)
**Trigger:** A sector ETF rises more than 25% in 30 calendar days.
**Override:**
- The easy money in that sector is done. New entries carry maximum mean-reversion risk.
- Existing positions in the sector: take partial profits (Minervini rule: 20–25% gain = partial exit)
- New entries: only on a pullback to a clearly defined support level with volume contraction, not at current highs
- Apply Marks second-level thinking: if everyone sees the same trade, the trade is crowded. Crowded trades unwind violently.

### Divergence 8 — Stagflation Signal
**Trigger:** Rising inflation data (CPI beat) combined with weakening economic data (PMI contraction, rising unemployment) in the same reporting period.
**Override:**
- Growth and cyclical stocks lose their fundamental support — avoid even if technically in Stage 2
- Commodity producers, energy infrastructure, and real assets outperform in stagflation (Dalio framework)
- Utilities face conflicting pressure: defensive appeal vs. rising input costs — require individual technical confirmation before recommending
- Bonds do not protect in stagflation — do not assume rate-sensitive sectors benefit from yield moves

---

## Report Settings

- **Securities to recommend:** 4 minimum (2 if Divergence 1, 2, or 5 is active)
- **Types:** Stocks and ETFs (at least 1 ETF per report for diversified exposure)
- **Market:** US-listed (NYSE, NASDAQ, AMEX)
- **Minimum average daily volume:** 500,000 shares (liquidity floor — no illiquid names)
- **Report timing:** Pre-market (before 9:30 AM ET)

---

## Account & Risk Parameters

Update these when account size changes.

- **Account size:** $50,000
- **Max risk per trade:** 1% of account ($500)
- **Max total portfolio risk (all open positions):** 4% of account
- **Max sector concentration:** 3 positions in any single sector
- **Position sizing formula:** (Account × Risk%) ÷ (Entry Price − Stop Price) = max shares
- **If stop distance exceeds 10% of entry price:** Flag it. At 1% account risk, a 10% stop on a $50 stock requires only 100 shares. Assess whether the position is meaningful enough to take.

---

## Sector Focus

These are the default priority sectors. Re-verify against current Stage analysis before applying.
If a sector not listed here is showing stronger RS and Stage 2 structure than these, include it.
This list is a starting screen, not a constraint.

**Priority sectors (as of 2026-06-29 — re-verify Stage 2 on charting platform before screening):**
- Nuclear Utilities (July 4th catalyst — reactors online, deregulation push; screen CEG, VST, SMR)
- Airlines / Transportation (gas tax suspension + WTI at $70; screen DAL, UAL, LUV, JBHT, ODFL)
- Financials (OBBB tax cuts favor domestically-focused large-cap; screen XLF components)
- Domestic Industrials (lower energy costs + tax cuts; screen XLI leaders by RS)

**Avoid or require elevated confirmation (as of 2026-06-29):**
- Energy (Divergence 3 active — WTI reversed 28% from March highs; suspend new longs)
- Consumer Discretionary (weak fundamentals, soft revenue trends — low consumer confidence offsets fuel tailwind; require full stack before entry)
- EM names including YPF (DXY strengthening — Divergence 4 watch)
- Technology (verify Stage 2 and Minervini template; recent chip weakness per June 25 session)

---

## Macro Context (Update Weekly)

This section is the human-written context layer. The report compares it against current
conditions and notes any divergence before applying it.

**Last updated:** 2026-06-29

- Market regime: Recovery/consolidation. S&P 500 ~7,413 as of June 29 (+17% from March low of ~6,343). Pulled back from June high of ~7,609; now testing 50-day MA (~7,363). 200-day MA ~6,925 — S&P comfortably above. 30-week MA not directly sourced — verify on charting platform (estimated ~7,000–7,100 given recovery trajectory). Broad market likely Stage 2 on weekly, but breadth is neutral/modest — monitor for Divergence 2 activation.
- Primary catalyst: Iran conflict ongoing. US-Iran strikes renewed June 29 near Strait of Hormuz. Oil bounced modestly on renewed supply fears but remains 28% below March highs. Conflict has not resolved — de-escalation remains the tail risk for energy names.
- Oil levels: WTI ~$70, Brent ~$72–73 (was WTI ~$98 / Brent ~$112 in March). **Divergence 3 is effectively active.** Oil has reversed 28% from conflict highs. Energy sector long thesis from March is largely invalidated. Suspend energy longs until WTI re-establishes above a clearly defined technical support level.
- Rate environment: 10-year Treasury yield 4.38% (as of June 26). Fed cuts still delayed — September 2026 is the current expectation. No rate relief yet. Rising yield environment remains a headwind for growth and high-multiple names.
- Dollar: DXY ~101.33. Up ~2.14% over the past month. Monitor weekly rate of change — Divergence 4 triggers if DXY moves >2% in any single 5-day period. EM names (YPF, etc.) carry elevated currency risk at current trajectory.
- Credit spreads: IG ~80 bps (near multi-decade tights), HY ~276–285 bps (as of June 24). Tightening — risk-on environment. Divergence 5 NOT active.
- VIX: ~18.41 (June 26 close). No elevated volatility. Divergence 6 NOT active. Standard stop distances apply.
- Risk posture: Selective. Broad market recovery intact above 200-day MA, but breadth is neutral and 50-day MA is being tested. Not a high-conviction momentum environment. Full 9-layer stack required — no shortcuts on Minervini template or multi-timeframe alignment.
- July 4th announcement context: Trump nuclear milestone — 2 of 3 experimental reactors already online (Antares Nuclear June 4, Valar Atomics June 18). Third expected by July 4. Gas tax suspension (18.4 cents/gallon gasoline, 24.4 cents diesel) actively being discussed — not yet law. OBBB tax cuts are already signed law — do not treat as new news; likely already priced in. Do not confuse "lower rates" with Fed action — no rate cut is imminent. "Lower fuel costs" refer to gas tax + energy deregulation, not WTI directly.
- Sector rotation update: Energy sector thesis from March invalidated by Divergence 3. Pivot screening focus: nuclear utilities (July 4 catalyst — verify Stage 2 on CEG, VST, SMR), airlines/transportation (gas tax suspension thesis — DAL, UAL, LUV), domestic financials and industrials (OBBB tax cuts). Consumer discretionary is lagging — weak revenue trends and soft consumer confidence offset the fuel tailwind. Verify all names against full Minervini template before entry.
- Primary tail risk: Iran escalation spike → oil reverses sharply upward → re-evaluate energy longs. Secondary risk: breadth continues to narrow while index holds → Divergence 2 activates → reduce to 2 recommendations, VCP base breakouts only.

---

## Full Technical Stack — Applied in Sequence

Every candidate must pass each layer. A failure at any layer ends the evaluation.

### Layer 1 — Weinstein Stage Analysis
- Price above 30-week MA (confirm current reading)
- 30-week MA flat or turning up
- Stock's RS vs. S&P 500 showing current leadership (not just recent — check today)
- The stock's sector must also be in Stage 2. A Stage 2 stock in a Stage 3 sector is a distribution trap.
- Volume behavior: volume must be contracting inside the base and expanding on the breakout

### Layer 2 — Minervini Trend Template (all 8 required — zero exceptions)
- Price above 150-day and 200-day MA
- 150-day MA above 200-day MA
- 200-day MA trending up for at least 1 month
- 50-day MA above both 150-day and 200-day MA
- Price above 50-day MA
- Price at least 25% above 52-week low
- Price within 25% of 52-week high (ideally within 15%)
- Relative strength rank above 70

### Layer 3 — Multi-Timeframe Alignment (Brown)
- Weekly chart must confirm Stage 2 structure before the daily chart is evaluated
- Weekly RSI must be in the appropriate regime range (bull: 40–90, bear: 10–60)
- Daily setup must align with weekly trend direction — a daily VCP inside a weekly downtrend is excluded

### Layer 4 — Entry Pattern (Minervini + Nison + Bulkowski)
In order of preference:
1. **VCP (Volatility Contraction Pattern):** Multi-week base with successively tighter price swings, volume drying up into the base, clear pivot point. Highest-probability entry.
2. **Base breakout on volume:** Price clears a defined resistance level on 2x or greater average volume. Confirm volume is genuine (not pre-market only).
3. **Momentum continuation near 52-week high:** Only valid if stop can be placed at a clean technical level within 6–8% of entry. Requires weekly RS rank above 80.

**Bulkowski checks for the specific pattern identified:**
- What is the historical success rate of this pattern type in the current market direction?
- What is the average gain of successful breakouts from this pattern?
- What is the throwback frequency? (How often does price return to test the breakout level before continuing — do not panic sell a throwback if it is within the expected range)
- What is the busted pattern scenario? If price breaks out and immediately reverses back through the base, note the potential short entry level and the magnitude of the typical busted-pattern move

### Layer 5 — Candlestick Confirmation (Nison)
Candlestick signals are only valid at significant technical levels.
Do not reference a pattern unless it appears at support, resistance, a base pivot, or a Fibonacci level.
Relevant confirmation signals at the pivot:
- Hammer, bullish engulfing, morning star, piercing line = bullish at support/pivot
- Shooting star, bearish engulfing, evening star, dark cloud = distribution warning at resistance
- Doji at resistance after a long run = possible exhaustion; do not add at this level

### Layer 6 — Fibonacci Levels (Brown)
- Identify the primary price swing (last major low to last major high)
- Key retracement levels: 38.2%, 50%, 61.8% — entries at these levels have higher probability
- Key extension levels: 127.2%, 161.8% — use as price targets alongside analyst targets
- If multiple Fibonacci levels cluster near the same price, that level has elevated significance

### Layer 7 — Oscillator Confirmation (Brown + Murphy)
Apply RSI market regime (identified in Step 0) before reading any oscillator.
- In bull regime: RSI pulling back to 40–50 on the weekly is a buy zone, not a warning
- In bear regime: RSI reaching 50 on the weekly may be near overbought
- MACD: Look for histogram turning positive or a signal-line cross above zero — confirms momentum, not entry alone
- Stochastics: Useful for identifying short-term exhaustion at resistance and oversold bounces at support

### Layer 8 — Fundamental Confirmation (Minervini)
For individual stocks only (not ETFs):
- Earnings estimate revisions: Have estimates moved up or down in the last 60 days?
- Analyst consensus: What is the average price target and current rating?
- Recent catalysts: Earnings beat, analyst upgrade, supply/demand development, insider buying?
- Zacks rank if available (Rank 1 or 2 preferred)
- Stocks with deteriorating fundamentals are excluded regardless of chart quality

### Layer 9 — Options Environment Check (Tastytrade / Cohen)
For the current environment, note IVR (Implied Volatility Rank):
- IVR above 50: Options premiums are expensive. If directional, consider debit spreads instead of outright calls to reduce premium paid. If non-directional, premium-selling strategies (cash-secured puts, covered calls) may offer better risk/reward than stock purchase.
- IVR below 25: Options cheap. Outright calls on high-conviction breakouts have lower premium cost relative to historical norms.
- In a geopolitical-driven high-volatility environment: buying outright calls on energy names likely means paying elevated IV — factor this into the trade decision.

---

## Pre-Trade Psychological Checklist (Douglas)

This is not optional. Complete before executing any recommended trade.

1. I have defined my exact stop price before entering. It is written down.
2. I accept that this trade can be a complete loss of my defined 1R risk. I have agreed to this before entering.
3. I will not move my stop to avoid a loss. The stop is the stop.
4. I understand this is one trade in a series of trades. The outcome of this single trade does not define my edge. My edge shows up over 20–30 trades.
5. I am not entering this trade because I fear missing out. I am entering because it passed the full stack.
6. If I am stopped out, I will not re-enter the same day out of frustration. I will evaluate the chart again the next session.
7. I am not trading with money I cannot afford to lose.

---

## Trade Journal Requirement (Tharp)

Log every trade as an R-multiple. This is how you verify whether you have a positive-expectancy system.

**Per trade, record:**
- Ticker, date, entry price, stop price, target price
- 1R = entry − stop (your defined risk unit)
- Outcome: actual exit price
- Result in R-multiples: (exit − entry) ÷ (entry − stop)
- Win or loss

**System-level tracking (every 20 trades):**
```
Expectancy = (Win% × Avg Winner in R) − (Loss% × Avg Loser in R)

Target benchmarks for this system:
- Win rate: 40–50% (Minervini-style momentum trading is not a high win-rate system)
- Average winner: 2R–4R (partial exits at 20-25%, runners held for 3R+)
- Average loser: 1R (stops respected = losers never exceed 1R)
- Target expectancy: +0.5R to +1.5R per trade
```

If actual expectancy falls below +0.3R over 20 trades, the system or the execution has a problem.
Identify which before adding capital or increasing position size.

---

## Marks Second-Level Thinking Check

Before finalizing any recommendation, answer:
- What is the consensus thesis on this trade? (What does everyone already believe?)
- Is that belief already reflected in the current price?
- What does the market expect that could be wrong?
- What is the asymmetric scenario — what would have to happen for this trade to produce a 4R+ outcome vs. a -1R outcome?
- If oil names are up 39% in 3 weeks, ask: who is not yet in this trade? If the answer is "everyone is already in," the risk/reward is unfavorable regardless of the technical setup.

---

## Special Instructions

One-off additions for the current period. Clear this section each weekly update.

**Active as of 2026-06-29:**
- Divergence 3 is in effect. Do not recommend new energy sector longs. Any existing energy positions: verify stops are tight; tighten to prior swing low or move to breakeven.
- Apply Marks second-level thinking before any July 4th trade: check RS trend for nuclear utility names over the prior 60 days. If a name has already run 25%+, the easy money is made — new entry requires pullback to defined support with volume contraction, not a chase at current highs.
- Gas tax suspension is not yet law as of June 29. Airline and trucking thesis depends on it passing. Flag this risk on any airline recommendation — the setup could reverse if the suspension fails legislatively.
- OBBB tax cuts are already signed law. Do not frame financials or industrials recommendations as "news plays" — they must pass the full technical stack on their own merits, not on announcement hype.
- Breadth is neutral with S&P testing its 50-day MA. If S&P closes below 50-day MA on above-average volume this week, treat as a distribution signal and reduce recommendations to 2 until breadth re-confirms.
- If DXY moves >2% in any single 5-day period, activate Divergence 4 immediately — remove or flag any EM or commodity-denominated name.
- Monitor oil daily. If WTI spikes >5% on a single session (Iran escalation), re-evaluate Divergence 3 status — energy longs may re-activate if oil reclaims prior support on volume.

---

## Report Output Format

Each recommended security must include all of the following. If any item cannot be
answered from current data, the security is not ready to recommend.

1. **Ticker and full name**
2. **Curriculum stack confirmation** — explicitly state pass/fail for Weinstein, Minervini (all 8), multi-timeframe alignment, entry pattern, and any Bulkowski pattern probability data
3. **Entry zone** — specific price range with rationale (base pivot, support level, etc.)
4. **Stop level** — specific price and technical reason (below base low, below support, below 50-day MA)
5. **Price targets** — near-term (Fibonacci extension or pattern-measured move) and extended (analyst consensus target). State source for each.
6. **Risk per share and R-potential** — calculated precisely
7. **Position size** — shares, calculated from current account settings
8. **Options note** — brief IVR comment and whether a spread structure is preferable to outright shares at current IV
9. **Divergence flags** — any active divergence rules affecting this security (oil reversal risk, dollar sensitivity, breadth conditions, etc.)
10. **Busted pattern level** — where does this setup fail, and what does that signal if it does?
11. **Advisor caveat** — the specific, named scenario that invalidates this trade, stated without hedging

---

Tags: #trading #swing-trading #criteria #report-config
