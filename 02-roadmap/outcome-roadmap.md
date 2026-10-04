# Outcome Roadmap & Trade-off Memo: Meridian Foundations

> Module 2 · Prioritization & Roadmapping for Product Leaders, ★ Deliverable 2
>
> Translate your strategy into a multi-team, outcome-driven roadmap, and a memo defending the hard prioritization calls behind it.

## 1. Outcome roadmap

_North star: foremen resolve RFIs through Meridian as easily as sending a text, and that field record becomes renewal proof for our 38 enterprise accounts. The full build is staged behind two gates, one behavioral and one financial. Dollar figures are illustrative, carried from the business case, since the brief provides no financials._

| Horizon | Outcome / bet | Owning team(s) | Success signal |
|---|---|---|---|
| Now (0 to 3 mo) | **Prove foremen will move RFIs out of calls and texts** (behavioral gate, 12-week pilot at two accounts, ~$0.46M) | Foundations: product, UX research, mobile engineering | At least 20% of pilot RFIs submitted through the app by week 12, with routing accuracy at or above 95% and offline sync performing; baseline RFI resolution times recorded in the first two weeks |
| Now (0 to 3 mo) | **Confirm the enterprise retention economics** (financial gate) | Finance, Customer Success, Foundations product lead | Real contract values, gross margins, and renewal risk confirmed for all 38 accounts; retention model clears a 24-month payback under the downside scenario |
| Now (0 to 3 mo) | **Protect near-term revenue at accounts already at risk** | Core Platform, Account Management | Renewal-risk drivers identified for the two at-risk accounts; Procore import/export restored for the two affected clients; dashboard request reviewed by the platform lead with retention context attached |
| Next (3 to 6 mo) | **Field RFIs route correctly and survive bad connectivity** (full build, released only if both gates pass, ~$1.54M) | Foundations: backend and systems engineering (after reallocation), mobile engineering | Routing accuracy at or above 95%, with low-confidence matches escalated to human review; offline sync success rate; first-session completion rate |
| Next (3 to 6 mo) | **Foremen receive answers, not confirmations** | Foundations | Median time from RFI submission to foreman notification of resolution falling against each project's own baseline |
| Next (3 to 6 mo) | **Executive reporting decided on the right roadmap** | Core Platform | Dashboard decision made and communicated to Enterprise Sales, with no Foundations capacity spent on it |
| Later (6 to 12 mo) | **RFI resolution through Meridian becomes the default across all 38 accounts** | Foundations, Customer Success (rollout and change management) | 40% of RFIs submitted and resolved through the app; 50% reduction in median submission-to-answer time against each project's baseline |
| Later (6 to 12 mo) | **Field gains become renewal proof** | Account Management, Customer Success, Finance | Renewal conversations at adopting accounts include RFI cycle-time improvements; retained gross profit tracked against the model |
| Later (6 to 12 mo) | **Earn the right to expand beyond RFI** | Foundations product lead, leadership | Deferred functions and phase-two candidates reconsidered only after routing accuracy and adoption thresholds are sustained |

https://claude.ai/artifact/UgFurrpyZPqeXNcX8a8Weq

## 2. Trade-off memo

_What did you sequence first, what did you push out, and what did you cut entirely, and why? Use WSJF / cost of delay reasoning where it helps._

**Illustrative WSJF scoring** (relative 1 to 5 scores, not sourced data; WSJF = cost of delay ÷ job size)

| Item | Business value | Time criticality | Risk reduction | Cost of delay | Job size | WSJF |
|---|---|---|---|---|---|---|
| Retention economics validation | 3 | 4 | 5 | 12 | 1 | **12.0** |
| 12-week behavioral pilot | 3 | 4 | 5 | 12 | 2 | **6.0** |
| Procore integration fix (#8) | 3 | 5 | 2 | 10 | 2 | **5.0** |
| Executive reporting dashboard (#10) | 3 | 4 | 1 | 8 | 4 | **2.0** |
| Full build (#7, #1, #9) | 5 | 2 | 2 | 9 | 5 | **1.8** |

> I chose to sequence the behavioral pilot and the retention economics validation first because they test the two assumptions the entire bet rests on: whether foremen will actually move RFIs out of calls and texts, and whether the 38 enterprise renewals are genuinely at risk. Both carry the highest cost of delay relative to job size. They are small, inexpensive pieces of work, and every quarter without their evidence risks committing $1.54M to the wrong build. I also sequenced near-term revenue protection first, the renewal diagnosis for two at-risk accounts and the Procore fix for two clients, because their cost of delay is measured in churn this quarter. I assigned that work to Core Platform and Account Management so revenue pressure is addressed without pulling Foundations off its focus.
>
> I pushed out the full build, the production foreman app (#7), offline-first reliability (#1), AI-assisted RFI drafting (#9), and RFI resolution notifications (#11, rescoped from schedule changes), because they are the largest pieces of work and their value depends entirely on assumptions the gates test first. Releasing them early would turn a capped $0.46M pilot into an uncapped $2.0M commitment. I pushed further out, behind a sustained performance threshold, photo markup (#2), daily log simplification (#4), and the four deferred enterprise functions: compliance, budget variance, document control, and multi-site coordination. Each would split a ten-person team before routing accuracy and offline reliability are proven world-class, and a team split five ways delivers five mediocre experiences.
>
> I cut entirely from Foundations the executive reporting dashboard (#10), the automated compliance checklist generator (#5), and the subcontractor portal (#14). Each is a legitimate, well-sourced enterprise request, and each pulls the team toward analytics and compliance depth rather than field adoption. The WSJF table makes the dashboard decision worth stating plainly: it scores slightly above the full build, because two renewals at risk give it real urgency. That is exactly why WSJF alone cannot set this roadmap. It measures urgency and size, not strategic fit. The dashboard belongs on the Core Platform roadmap, where its cost of delay can be weighed against that team's priorities, not inside the one initiative built to win the field. I also cut the multi-project dashboard migration (#3), weather integration (#6), time tracking (#12), and the web UI refresh (#13), because none of them moves the RFI north star.

## Link to full artifact

https://github.com/BT-Product/product-leadership-final/blob/main/02-roadmap/plc-m2-lab.md
