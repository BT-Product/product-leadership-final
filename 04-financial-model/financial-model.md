# Financial Model: Meridian Foundations

> Module 5 · Master Product Financials & Strategic Bets, ★ Deliverable 5
>
> The business case for funding your bet, and the explicit kill criteria that would tell you to stop.

## 1. Business case

_Why this initiative is worth funding over the alternatives. Include the key unit economics assumptions, CAC, LTV, payback period, where relevant._

_This is a retention bet inside existing accounts, not an acquisition bet, so the model measures retained gross profit rather than LTV:CAC. Only the 38 accounts come from the brief. Every other figure is illustrative and labeled, since the brief provides no contract values, margins, churn rates, or costs._

| Assumption | Value | Source / rationale |
|---|---|---|
| CAC | Not applicable | All 38 accounts are existing customers, so there is no acquisition cost. The relevant investment is product development to preserve contracts |
| LTV | Illustrative base: ~$8.0M per account at 10% annual non-renewal risk, rising to ~$13.3M if risk falls to 6% | $1.0M contract × 80% gross margin ÷ non-renewal rate. Shown for context only; retained gross profit below is the primary metric |
| Payback period | Base: ~34 months against a 24-month hurdle. Downside and severe downside: never | $2.0M investment ÷ $716K annual net retained gross profit. 24-month hurdle recommended because returns arrive at renewal, likely year two, so 18 months would fail on timing alone |
| Investment required | ~$2.0M: $0.46M for a 12-week pilot, $1.54M for the full build, plus ~$0.5M a year to run | Illustrative: ten-person team at $200K fully loaded each. Funding is staged, only the pilot is requested now |
| Expected return | Base: $1.22M retained gross profit a year ($716K after run costs). Downside: $374K. Severe downside: $53K | 38 accounts × contract value × gross margin × baseline non-renewal risk × risk reduction. Counts only the renewal risk the app removes, not full contract value |
| Accounts in scope | 38 | Sourced from the brief: Meridian is the system of record for 38 of the top 100 US construction firms |
| Average annual contract value | Base $1.0M · Downside $750K · Severe $500K | Illustrative. To be replaced with confirmed figures from Finance before the full build decision |
| Gross margin | Base 80% · Downside 75% · Severe 70% | Illustrative |
| Baseline annual non-renewal risk | Base 10% · Downside 7% · Severe 4% | Illustrative. The brief confirms mid-market churn, not enterprise churn, which makes this the most financially load-bearing assumption |
| Reduction in non-renewal risk from field adoption | Base 40% · Downside 25% · Severe 10% | Illustrative. A 24-month payback in the base case requires roughly a 50% reduction |

> **The case in one paragraph:** Field teams at our 38 enterprise accounts barely use Meridian, so RFIs travel by call and text, crews wait, and our platform misses what happens on site. We are betting that a lightweight, offline-first foreman app will move 40% of field RFIs into Meridian within a year and cut question-to-answer time in half, turning faster field answers into renewal proof that GC executives can see. The return is retention, measured as retained gross profit: contract value × gross margin × baseline non-renewal risk × the risk the app removes, across 38 accounts. Under illustrative assumptions, the base case preserves about $1.22M in gross profit a year, but pays back in roughly 34 months, short of a 24-month hurdle, and both downside cases never pay back. The full build therefore only makes financial sense if these accounts carry meaningful renewal risk, around 10% a year on roughly $1M contracts, and field adoption cuts that risk roughly in half. That is why we are funding the $0.46M pilot only, with the $1.54M full build released behind a behavioral gate and a financial gate. If confirmed figures fall short, the initiative is redesigned at lower cost or brought to the board explicitly as strategic defense of our complexity premium, not presented as a self-funding retention investment.

## 2. Kill criteria

_The specific signals that would tell you this bet is no longer worth pursuing. Be explicit about the metric, the threshold, and the timeline._

**Gate 1: Behavioral**

> If **the share of RFIs at the two pilot accounts submitted through the app** does not reach **20%, while routing accuracy holds at or above 95% and offline sync performs as designed,** by **week 12 of the pilot**, we will **stop the bet: the $1.54M full build is not released, the team reallocation to backend and systems engineering is not committed, the pilot app stays live in maintenance only, and the team runs a six-week diagnostic on whether trust, not friction, is the barrier.**

**Gate 2: Financial**

> If **the retention model, rebuilt with confirmed contract values, gross margins, and renewal risk for the 38 accounts,** does not reach **a 24-month payback under the downside scenario** by **the full build decision at the end of the pilot**, we will **withhold the $1.54M full build and either redesign the initiative at lower cost or bring it to the board explicitly as strategic defense.**

**Product underperformance clause**

> If **routing accuracy falls below 95% or offline sync fails** during the pilot, the behavioral test is invalid, not failed. The team gets **four weeks** to fix the product and **one rerun** of the 12-week measurement. A second product failure triggers Gate 1's consequences.

_Decision owners: the Foundations product lead calls Gate 1 at the week-12 review. Leadership and the CFO call Gate 2 on the product lead's recommendation. Neither gate is put to a vote._

## Link to full artifact

https://github.com/BT-Product/product-leadership-final/blob/main/04-financial-model/plc-m5-lab.md
