---
name: design-evolving-systems
description: Draft (beta). Collaboratively design a system and the way people and agents will build and evolve it. Use for early system design, choosing methods or technologies from prior art, or revisiting a design in light of feedback.
---

# Design evolving systems

> [!IMPORTANT]
> **DRAFT · BETA** — This skill is under active development. Its design process may change with field experience.

Start with the decision the user faces. Work through a concrete case together. Offer a provisional interpretation they can correct, and ask the question whose answer would most change the design. Use the stages below as moves in a conversation. Enter wherever the user already has evidence and return to earlier choices when an assumption changes. Let the user decide when a sketch, decision note, or other artifact would help.

## 1. Establish the vision

Ask who needs what to change and why it matters. Walk through an occasion when that person would use the system. What happens today? What would they be able to do differently? Who else experiences the consequences? Use their answers to locate the boundary of the undertaking and recognize success in practice. Keep candidate products out of the vision. If a technology is already mandated, carry it forward as a constraint.

For the system that will build or change this one, ask a second question: who will notice that a design decision needs revisiting, and what will they need in order to act? The two purposes can differ. A booking system allocates places. The people changing its allocation policy need to understand who is being left out.

## 2. Find the functional structure

Follow the same case from trigger to outcome. Name each essential responsibility in domain language, such as “recognize an eligible request” or “resolve competing claims.” Locate who has authority, what knowledge passes between responsibilities, and what happens when a usual assumption fails. A responsibility may belong to a person, an agent, software, or an existing institution. Leave that allocation open when it has no bearing on the decision.

Try a second case where the boundary is uncertain. Split or combine responsibilities if doing so explains a real difference in behavior or ownership. Stop when you and the user can reason about the important choices. Stakeholder scenarios and logical decomposition are established starting points for these first two moves. [NASA Systems Engineering Handbook, §§4.1 and 4.3](https://www.nasa.gov/reference/4-0-system-design-processes/)

## 3. Find a method that earns its place

Turn the hardest uncertainty into a research question. Is the team unsure what people need, what a domain term means, what it is allowed to do, or whether anyone has tried a fundamentally different approach? Search for prior work on that question. Look in adjacent domains when the local literature takes an assumption for granted. Consult original method descriptions and accounts of comparable use. Explain which part transfers, where the analogy breaks down, and which claim is still a hypothesis. For legal constraints, establish the relevant jurisdiction and check the governing source.

Compare promising methods with the simplest credible way to proceed. Competing meanings might warrant a conversation with domain experts, domain-driven design, or an ontology, depending on who needs shared meaning and what they must do with it. An unsettled market calls for evidence from users. A novel concept that familiar solutions keep crowding out may warrant C–K exploration. A hard group decision might benefit from a design sprint. Combine methods when each resolves a distinct uncertainty. Identify who contributes knowledge, who can challenge it, and who decides. [Hatchuel and Weil on C–K theory](https://doi.org/10.1007/s00163-008-0043-4)

For each selected method, decide with the user where it belongs. It can guide a single conversation, become a recurring design practice, or become a capability of the system itself. For example, try C–K in a workshop first. If later decisions depend on reopening branches when knowledge changes, consider keeping concepts, evidence, and their relationships editable. Work out whether a new observation should revise one branch or prompt a fresh pass. A shared record of the reason for one decision may be enough.

## 4. Choose technologies against those needs

Translate the chosen approach into a capability someone will actually use. “When evidence changes, find the decisions that depend on it” gives you grounds to compare linked notes, a table, and a knowledge graph. Ask what each would let the team do on a real case, who would maintain it, and how hard it would be to change course. A graph database, an ontology language, and a dashboard serve different purposes. Select each only when its contribution is clear. If the team needs to derive several realizations from one stable model, consider [OMG’s Model Driven Architecture](https://www.omg.org/mda/).

Check current documentation for decisive capabilities and look for maintained deployments in comparable settings before claiming maturity. Explain the strongest reason for a choice and what evidence would reverse it. Defer the choice when the distinction has no consequence yet.

## 5. Enter implementation when it helps decide or build

Stay at the user's chosen depth. When a major choice rests on feasibility, suggest the smallest walkthrough or experiment that could distinguish the options. Move into implementation details when the user wants to build or when a particular detail could overturn the design. Return what was learned to the relevant earlier decision.

## Close the feedback loop on every pass

While considering a change, name the outcome you expect and how someone could observe it. Use a real case, a conversation, or an existing signal when possible. Agree who can interpret the evidence, when it warrants attention, and who can decide to keep, revise, or retire the change. After acting, compare the next observation with the expectation. Look for effects on people beyond the immediate user. This adapts the [Model for Improvement and its Plan–Do–Study–Act cycle](https://www.ihi.org/library/model-for-improvement).

Ask where the feedback points. If a team repeatedly gets an elaborate report when it needs a design conversation, the design method itself needs attention. If people can follow the method but the resulting system fails them, reopen the assumption or functional choice implicated by that experience. Carry forward decisions whose reasoning still holds. Where others will need to pick up the work, use their existing medium to retain the decision, its reason, and what would reopen it.

Use the same discipline when changing this skill. Trace a correction to the instruction that shaped the decision, try the smallest useful revision, and revisit its effect on a subsequent case. End the current pass when the decision is clear enough to act on or the next observation depends on real use.
