# Team Charter: Meridian Foundations

> Module 3 · Lead and Develop High-Performing Teams, ★ Deliverable 3
>
> Define how your team operates. Two completed components: **What We Own** and **How We Decide**.

_Team: 10 people across product, mobile engineering, backend and systems engineering (reallocated from mobile), UX research, and customer success._

## 1. What We Own

_The team's mandate: the outcomes and surfaces this team is accountable for end-to-end, and the explicit edges where your ownership stops._

| Area | We own it | We influence it (don't own) |
|---|---|---|
| **Field surface** | The foreman-facing RFI app end to end: capture, submission, first-run experience, and receiving resolutions | The PM web app and the core Meridian platform, owned by Core Platform |
| **RFI routing** | The logic that maps a field-captured RFI to the right approval chain for each project and firm, including human review of low-confidence matches | The core data model and each firm's enterprise configuration, owned by Core Platform. We can request changes, not make them |
| **Offline reliability** | Store-and-forward, retry, and sync behavior on the device, tested for job-site conditions | The underlying notification infrastructure, bought from a vendor we select and manage but don't build |
| **Field adoption outcomes** | KR1 to KR3: RFI share through the app, routing accuracy, and submission-to-answer time | How answers are written and how fast responders decide. PMs, engineers, and architects own the content of a resolution, we own its delivery |
| **Pilot and behavioral gate** | Pilot design, account rollout, baseline measurement, and the week-12 kill decision | Pilot account selection, shared with Account Management, who owns the client relationships |
| **Full build funding** | The recommendation and the behavioral evidence behind it | The financial gate and budget release, owned by Finance and leadership |
| **Enterprise renewals** | Field results that make renewal conversations stronger | Renewal outcomes, owned by Account Management and Enterprise Sales |
| **Enterprise depth** | A guarantee that nothing we ship removes or degrades features finance and compliance teams use | Those features themselves, and any request to expand them, including the executive dashboard, owned by Core Platform |

> Our mission in one line: Get every foreman an answer as fast as sending a text, and turn that answer into a record the whole enterprise can trust.

## 2. How We Decide

_The team's decision-making operating model: the decisions you make, who makes each call, and how disagreements resolve._

| Decision type | Who decides | Who's consulted | How we break a tie |
|---|---|---|---|
| **Scope: what's in or out of the RFI workflow** | Foundations product lead | UX research, engineering leads, foreman panel | Test against the where-to-play statement and the hard no. If still split, the product lead decides and the team commits |
| **Technical approach: routing, offline sync, build vs buy** | Backend and systems engineering lead | Product lead, mobile engineering, Core Platform architects | Engineering lead owns the "how." If the choice changes scope or timeline, it moves to the product lead |
| **First-run and capture experience** | UX research and design lead | Foreman panel, product lead, mobile engineering | Field evidence wins. If there's no evidence yet, test both with foremen before deciding. If time forces a call, the product lead decides |
| **Week-12 pilot gate** | Foundations product lead | Engineering leads, UX research, customer success | No tie to break. The pre-committed threshold decides: under 20% of pilot RFIs through the app, with the product performing, stops the bet |
| **Releasing the full build** | Leadership and the CFO, on the product lead's recommendation | Finance, customer success, Account Management | The retention model decides: the full build proceeds only if it clears a 24-month payback under the downside scenario using real data |
| **Feature requests from outside the team** | Foundations product lead | The requester, Account Management, Core Platform | Requests outside RFI scope are declined or routed to their owning team. If the requester disagrees, it goes to the quarterly leadership guardrail review, and the current call holds until then |
| **Changes touching the core data model** | Core Platform | Foundations backend and systems engineering lead | Core Platform holds the veto. Enterprise contracts are non-negotiable, so protecting finance and compliance features beats our speed |
| **Team composition and reallocation** | Foundations product lead, with the engineering manager | Leadership | Escalate to the quarterly leadership guardrail review. Drift back toward a mobile-heavy team is flagged there, not resolved informally |

> Our default: the owner of each decision type decides, the product lead on what and why, engineering on how, design on experience, with field evidence beating opinion whenever we have it; we escalate to the quarterly leadership guardrail review when a decision would change our scope, cross the hard no, touch features finance and compliance teams depend on, or move people across team lines.

## Link to full artifact

https://github.com/BT-Product/product-leadership-final/blob/main/03-team-charter/plc-m3-lab.md
