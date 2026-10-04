# Product Strategy One-Pager & OKRs: Meridian Foundations

> Module 1 · Craft an Advanced Product Strategy, ★ Deliverable 1
>
> Your one spine: the **Playing to Win** cascade, one deliberate **hard no**, and an **OKR cascade** that flows directly from it.
> Draft the cascade + hard no in Sprint 1, then add the OKRs in Sprint 2. The goal: specific enough that a skeptical board member couldn't poke a hole in it.

## 0. Chosen scenario

**Path:** Meridian Foundations (B2B · adoption + expansion)

I chose Meridian because I'm currently in the real estate space building a platform that helps real estate agents provide a world class experience when their clients need to buy and sell a property at the same time. Meridian scenario gave me the extra product thinking experience I need to excel.

## 1. Playing to Win cascade

| Question | Your choice |
|---|---|
| **Winning aspiration**: winning in the customer's terms, not internal metrics | We win when a foreman or superintendent can send what's happening on site and get back what he needs to keep working, an answer, a status, a decision, as fast and as easily as sending a text. Project managers and finance win by inheriting a live, accurate record of the job site instead of a text thread they were never part of. |
| **Where to play**: segment, geography, channel, use case (the no's matter too) | We play inside our 38 existing top-100 enterprise accounts, not the broader top-100 market, on the job sites where our contracts already run. We focus on one use case: the foreman and superintendent RFI workflow, submitting RFIs and receiving resolutions through a lightweight, purpose-built mobile view, not a scaled-down version of the full platform. Budget variance, compliance, document control, multi-site status, the broader top-100 market, and mid-market accounts are explicitly out of scope for this phase. |
| **How to win**: your differentiator competitors can't easily replicate | A competitor can build a clean RFI capture app. None of them can correctly route it, track it against this project's specific approval chain and compliance obligations, or notify the foreman the instant a real answer exists, because that requires already being the system those approvals and obligations live in. That account depth compounds over the life of each relationship rather than being a fixed target a competitor could catch up to once. We win by making capture as easy as a text and everything after capture invisible and automatic, because we're the only ones who already know where it needs to go, and we keep knowing more. |
| **Capabilities required**: what you must be world-class at (build / buy / partner) | We must be world-class at two things. **Routing accuracy (build):** correctly mapping a captured RFI to the right approval chain for the specific project and firm, with any low-confidence match escalated to human review rather than routed silently. **Offline-first reliability (buy the notification infrastructure, build the offline behavior):** a submitted RFI and its returning answer survive poor or intermittent job-site connectivity through store-and-forward and retry logic, engineered and tested for construction-site conditions. Capture UX must clear a simple first-use bar, but it is not the moat. Our team of 10 was sized for a broader mobile build, so we reallocate within it: fewer mobile engineering seats, added backend and systems engineering depth. |
| **Management systems**: the metrics and rituals that reinforce your choices | We track median submission-to-notification time, routing accuracy, and offline sync success rate as proof the winning aspiration is real, and first-session completion as the adoption gate it depends on. Guardrails, reviewed quarterly with leadership, confirm team composition is held to its backend-and-systems reallocation, and that no deferred function is reconsidered until a defined performance threshold on routing accuracy and adoption is met. A recurring foreman panel keeps the team anchored to real field friction, and a monthly engineering review protects the two capabilities the strategy depends on. |

## 2. Your one hard no

_One valuable thing you are explicitly choosing **not** to do, and why it protects the focus of everything above. This is a deliberate trade-off, not a backlog of deprioritized items._

> We will not build parity across Meridian's other enterprise functions, compliance, budget variance, document control, and multi-site coordination, in this phase, even though enterprise sales and clients with renewals at risk are actively asking for them, because collapsing our full team's focus onto a single workflow is what makes routing accuracy and offline reliability world-class rather than merely adequate. A team split five ways delivers five mediocre experiences. A team aimed at one delivers something a foreman actually trusts.
>
> Refinement: we will not build document control as a standalone capability. An RFI resolution may include an attached drawing, spec, or document as part of its answer. That is not document control, it is a complete response.

## 3. OKR cascade

_One Objective and three Key Results that flow directly from the cascade. Each KR must be a measurable **outcome**, not an output/milestone._

> **Objective:** Make Meridian the first place a foreman turns to resolve an RFI, without sacrificing the routing accuracy enterprise teams depend on.
>
> - **KR1:** Share of RFIs submitted and resolved through the field app, rather than calls or texts, from near-zero (field teams barely use the platform today, per Meridian's own data) to 40% across RFI-enabled projects by 12 months after launch. A first milestone toward majority adoption, not the end state.
> - **KR2:** Automated routing accuracy, RFIs correctly mapped to the right approval chain with no manual PM correction, from no current capability to 95% or higher by 12 months after launch, with every lower-confidence match escalated to human review rather than routed silently.
> - **KR3:** Median time from RFI submission to foreman notification of resolution, measured end to end, from each project's own pre-Foundations baseline (recorded during the pilot) to 50% lower by 12 months after launch.

_Targets are deliberate stretch choices, not sourced figures. KR1 and KR3 activate only if the 12-week behavioral pilot passes its gate._

## 4. AI pressure-test notes

_Run the devil's-advocate prompt (in the Sprint 2 guide). Capture the verdict._

| Prompt question | What the AI surfaced | Change or defend? |
|---|---|---|
| Biggest assumption that could be wrong | That foremen avoid Meridian because RFIs are cumbersome, not because they trust a person ("Mike answers him") more than a system. If wrong, routing, offline sync, and notifications get built for a behavior that never arrives. | **Change.** Added a 12-week behavioral pilot at two accounts before the full build, with a kill criterion that separates "the product failed" from "the hypothesis failed." Added a design test: notifications name the person who resolved the RFI, preserving human trust rather than engineering around it. |
| The board question I can't yet answer | What observed behavioral evidence, not interviews or stated preference, shows foremen will move RFIs into Meridian if it becomes as easy as texting? | **Change.** The pilot exists to answer this. Full build funding is released only after the behavioral gate passes. |
| KRs that are outputs in disguise | No pure outputs, but KR2 measures whether the machine works rather than customer value, 95% accuracy means 1 in 20 RFIs misrouted in a trust product, and KR3 started its clock at "answer available," so it could be hit while RFIs still take days. | **Change.** KR3 now measures end to end from submission. KR2 adds human review for low-confidence matches, so failures become flagged second looks instead of silent errors. **Defend** KR2 as a valid KR: routing accuracy is the moat, and if it slips, the "invisible and automatic" promise breaks. |
| The "no" I should reconsider | Document control: an RFI resolution may point the foreman to a drawing or spec, so a categorical exclusion could block what a complete answer needs. Suggested allowing a thin slice "whenever it improves the RFI workflow." | **Partially change.** Kept document control out as a standalone capability, but allowed RFI resolutions to carry attachments. **Defend** against the open-ended "whenever it helps" wording, which would let scope creep back in. |
| Strategy or wish list? Why? | A strategy: it makes real choices about customer, workflow, capabilities, resources, and what it won't do. But it rests on an unvalidated behavioral assumption, and two KRs prove the plumbing works rather than proving customer outcomes. | · |

## 5. Self-diagnostic (6 questions)

- [x] **Clear**: a new PM could read it and know exactly what we will and won't do. One segment, one workflow, one surface, and an explicit list of what's out.
- [x] **Names the real challenge**: the diagnosis is specific enough to be uncomfortable. The platform's own frontline users route around it, and the strategy admits its core behavioral assumption is unproven.
- [x] **Makes a hard bet**: it says no to something valuable. Four enterprise functions requested by sales and clients with renewals at risk.
- [x] **Cascadable**: teams can translate it into their own OKRs. Each KR maps to a cascade box: KR1 to the winning aspiration, KR2 to how to win, KR3 to offline-first reliability.
- [x] **Coherent**: every choice reinforces the others. RFI-only scope protects the two world-class capabilities, which deliver the moat, which keeps the winning aspiration's promise.
- [x] **Committed**: resources are actually moving toward it. The team of 10 reallocates toward backend and systems engineering, staged behind the pilot gate so commitment follows evidence.

## Link to full artifact

https://github.com/BT-Product/product-leadership-final/blob/main/01-strategy/plc-m1-lab.md
