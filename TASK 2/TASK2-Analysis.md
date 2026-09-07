# Task 2 — Partner Economics Analysis

This analysis is based only on the supplied Excel file. I used the `Data` sheet for traffic and registration-level checks, and the values provided in the task for payouts, ARPU/ARPPU and return multipliers.

## Quick decision

| Campaign | Landing CVR | Affiliate ROI | Zimran 6M ROI | Decision |
|---|---:|---:|---:|---|
| Partner #1 — Desktop | 10.18% | +10.84% | -11.12% | Optimize before scaling |
| Partner #1 — Mobile | 8.28% | -21.12% | +117.30% | Keep; fix partner economics |
| Partner #2 — CPC | 15.07% | +43.48% | +2.42% | Keep as a controlled test; improve margin |

The main takeaway is that conversion rate alone gives the wrong ranking. Partner #1 Mobile has the lowest landing-page conversion, but it has the best projected economics for Zimran. Partner #2 has the best conversion, while Zimran is only slightly above break-even.

---

## 1. Why do landing-page conversions differ?

Landing-page conversion is:

**registrations / clicks**

- Partner #1 Desktop: 353 / 3,467 = **10.18%**
- Partner #1 Mobile: 333 / 4,020 = **8.28%**
- Partner #2: 1,127 / 7,479 = **15.07%**

I would not claim one exact cause from this dataset, because it does not include ad creatives, placements, audiences, landing-page versions or campaign settings. What the data does show is that the difference is not only caused by country mix.

For example, Partner #2 converts better in several of the largest countries:

| Country | P1 Desktop | P1 Mobile | P2 |
|---|---:|---:|---:|
| United States | 7.99% | 6.72% | 13.67% |
| United Kingdom | 11.21% | 9.77% | 18.41% |
| Canada | 8.50% | 6.53% | 11.45% |
| Australia | 16.98% | 11.92% | 16.95% |

New Zealand is an exception: P1 converts better there, but the sample is much smaller for P1.

Device-level data points in the same direction. P1 Mobile converts at **8.92% on Android** and **6.76% on iOS**, while P2 converts at **17.55% on Android** and **17.04% on iOS**. That suggests the gap is not simply “mobile users convert worse.”

There is also an important difference after registration.

### Registration → qualified lead

- P1 Desktop: 326 / 353 = **92.35%**
- P1 Mobile: 317 / 333 = **95.20%**
- P2: 911 / 1,127 = **80.83%**

Partner #2 gets more registrations, but a larger share of them fails the lead criteria. In the raw data, **all 216 non-qualified P2 registrations are under age 35**. I did not find country or gender failures among P2 registrations.

Even after that leakage, P2 still produces the most qualified leads per click:

- P1 Desktop: **9.40%**
- P1 Mobile: **7.89%**
- P2: **12.18%**

So I would describe P2 as **high-converting traffic with weaker age qualification**, not simply “low-quality traffic.”

### What I would check next

If I had campaign metadata, I would compare creative, placement, audience targeting and landing-page variant. With the current data, the first useful cuts are country, OS/device and age.

---

## 2. Is it profitable for the affiliates to keep sending traffic?

This question should be answered from the partner's point of view: affiliate income versus the media budget they spent.

### Partner #1 — Desktop

- Ad budget: **$2,647.01**
- Affiliate income: **$2,934.00**
- Profit: **+$286.99**
- ROI: **+10.84%**

**Yes.** The desktop campaign is profitable for Partner #1 at the current $9 CPA.

### Partner #1 — Mobile

- Ad budget: **$1,406.64**
- Affiliate income: **$1,109.50**
- Profit: **-$297.14**
- ROI: **-21.12%**

**No, not under the current setup.** Partner #1 should either improve the mobile campaign or stop sending mobile traffic at a $3.50 CPA.

Its current media cost per lead is:

**$1,406.64 / 317 = $4.44**

That means $3.50 per lead is below the partner's break-even point.

### Partner #2 — CPC

- Ad budget: **$1,720.17**
- Affiliate income: **$2,468.07**
- Profit: **+$747.90**
- ROI: **+43.48%**

**Yes.** Partner #2 has the strongest affiliate-side economics.

---

## 3. Which campaigns should Zimran keep?

For Zimran, the decision is different. I use projected six-month income versus traffic cost, as required in the task.

### P1 Desktop — optimize / pause scaling

- Projected 6M income: **$2,607.61**
- Traffic cost: **$2,934.00**
- Zimran ROI: **-11.12%**

At the current $9 CPA, Zimran loses money.

The useful part is the break-even comparison:

- Partner break-even CPA: **$8.12**
- Zimran break-even CPA: **$8.00**

There is no win-win payout at the current performance, but the gap is very small. Only about **$39** separates the two break-even totals, or roughly **1.5%**.

So I would **not kill the campaign immediately**. I would stop scaling it and run a short optimization test. A ~1.5% improvement in media efficiency or downstream value is enough to create room for both sides to be profitable.

### P1 Mobile — keep, but make it sustainable

- Projected 6M income: **$2,410.92**
- Traffic cost: **$1,109.50**
- Zimran ROI: **+117.30%**

This is Zimran's best campaign by a large margin.

The problem is that the affiliate loses money. If nothing changes, the partner has no reason to keep supplying the traffic.

Break-even CPA:

- Partner: **$4.44**
- Zimran: **$7.61**

That leaves a wide range where both sides can make money.

A practical test would be a **$4.50 CPA**:

- Partner income: 317 × $4.50 = **$1,426.50**
- Partner ROI: approximately **+1.4%**
- Zimran projected ROI: approximately **+69.0%**

I would start around $4.50 rather than jumping much higher, then watch volume and cohort quality.

### P2 CPC — keep, but do not scale blindly

- Projected 6M income: **$2,527.77**
- Traffic cost: **$2,468.07**
- Zimran ROI: **+2.42%**

By the task rule, ROI is above zero, so the campaign should continue. But the safety margin is only about **$60** on this traffic volume.

Zimran's break-even payout is approximately:

**$2,527.77 / 7,479 = $0.338 per click**

The current payout is already **$0.33**, so there is very little room for performance to deteriorate.

At the same time, Partner #2 buys traffic for $0.23/click and earns +43.48% ROI. That gives Zimran room to negotiate.

At a **$0.30 payout**:

- Partner ROI would still be about **+30.43%**
- Zimran traffic cost would fall to **$2,243.70**
- Zimran projected ROI would rise to about **+12.66%**

I would test a lower payout before increasing volume.

---

## 4. Concrete optimization actions

### P1 Desktop

The issue is not conversion alone; it is that total user value is slightly below what both sides need.

1. **Pause scaling and optimize for a small efficiency gain first.** The joint break-even gap is only ~1.5%.
2. **Lower media cost per qualified lead.** Test audiences, placements and creatives on the affiliate side.
3. **Improve post-registration monetization.** Even a small increase in 6M value would move Zimran above break-even.
4. **Then renegotiate CPA.** A payout cut without better campaign economics just moves the loss from Zimran to the affiliate.

### P1 Mobile

Here the traffic is very valuable to Zimran, but the partner cannot sustain it.

1. **Test CPA around $4.50–$5.00** instead of $3.50.
2. **Keep the test controlled by cohort.** A higher payout may bring more volume but not necessarily the same quality.
3. **Work on mobile conversion.** P1 Mobile has the lowest landing CVR (8.28%), so improving the funnel creates extra room for both sides.
4. **Track cost per qualified lead, not CTR alone.**

Another route would be to keep the $3.50 CPA and make the campaign much more efficient, but at the current budget the partner would need roughly **402 leads instead of 317** to break even — about **27% more**. That is a much larger change than a modest payout adjustment.

### P2 CPC

Because Zimran pays per click, wasted clicks matter directly.

1. **Test a CPC payout around $0.30.**
2. **Tighten age targeting toward 35+.** The clearest leakage in the registered P2 cohort is age: 216 registrations fail only because they are under 35.
3. **Segment P2 by device and country.** Keep the segments with the best downstream value rather than optimizing only for CTR.
4. **Set a minimum ROI buffer before scaling.** +2.42% is technically positive, but too thin to treat as a strong win.

---

## 5. How would Table 1 optimization affect Table 2?

The two tables are two sides of the same transaction.

If Zimran **raises the payout**:
- partner income and ROI improve;
- Zimran traffic cost increases;
- Zimran ROI decreases.

If Zimran **lowers the payout**:
- Zimran ROI improves;
- partner ROI falls.

That is why the goal should not be to maximize either table independently. The goal is to find a range where both sides want to continue.

Two examples show the trade-off clearly:

| Campaign | Change | Affiliate ROI | Zimran 6M ROI |
|---|---|---:|---:|
| P1 Mobile | CPA $3.50 → $4.50 | ~+1.4% | ~+69.0% |
| P2 CPC | payout $0.33 → $0.30 | ~+30.4% | ~+12.7% |

P1 Desktop is different: changing the payout alone cannot currently make both sides profitable. First, the underlying economics need to improve by roughly 1.5%.

---

## Final recommendation

**Partner #1:** keep the relationship, but manage desktop and mobile differently. Desktop should not be scaled until economics improve slightly. Mobile is highly profitable for Zimran, so I would raise the payout enough to make it sustainable for the affiliate and then test whether the extra volume keeps the same quality.

**Partner #2:** keep it, because projected Zimran ROI is positive, but treat it as an optimization case rather than a scaling case. The affiliate has plenty of margin while Zimran is close to break-even, so payout renegotiation and tighter 35+ targeting are the first moves I would test.

The broader lesson from the dataset is simple: **the highest conversion rate is not automatically the best business outcome.** I would make decisions on qualified traffic, long-term user value and two-sided unit economics rather than CTR or landing CVR in isolation.

---

## Assumptions and checks

- Lead definition used: registered user, male, age 35+, and country in the United States, Canada, United Kingdom, Australia or New Zealand.
- Desktop return multiplier: **8.3×**.
- Mobile return multiplier: **4×**.
- P2 has one combined ARPU ($0.33), so its six-month income is estimated by splitting its 1,127 registrations by OS:
  - **733 desktop**
  - **394 mobile**
- Desktop OS classification: macOS, Windows variants and Linux.
- Mobile OS classification: Android, iOS, Windows Phone and Blackberry.
- P2 projected 6M income:
  **$0.33 × (733 × 8.3 + 394 × 4) = $2,527.77**
- The 7 / 4 / 12 paying-user counts are inferred from rounded ARPU and ARPPU values, so they should be treated as approximate.
- The raw data contains **14,966 unique clicks** and **1,813 unique registered profiles**; no duplicate click IDs or profile IDs were found.
- This file does not make causal claims about creative or landing-page performance because those campaign-level fields are not present in the supplied data.
