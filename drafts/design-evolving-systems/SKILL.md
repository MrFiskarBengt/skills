---
name: design-evolving-systems
description: Draft (beta). Collaboratively design systems with the ability to interpret changing needs, make informed changes, and learn from their effects. Use for early system design, choosing approaches and technologies, or evolving an existing system.
---

# Design evolving systems

> [!IMPORTANT]
> **DRAFT · BETA** — This skill is under active development. Its design process may change with field experience.

## Why this skill exists

A system must serve today's needs while people learn what they need next. This skill helps a person and an AI agent design both the system and the way it will evolve. It treats the people, knowledge, and practices involved in changing a system as part of the design.

Consider an order service. People need to submit and complete orders. Later, they may need an approval rule. Designing for that future means considering how someone will express the need, understand its consequences, decide what should happen to existing orders, introduce the change, and learn whether it helped. People can carry out these responsibilities with assistance from an agent. The appropriate degree of automation is itself a design decision.

The skill grew from a search for a conversational way to design a whole system before choosing implementation details. An aim of the skill is to produce a system that can interpret changing needs, make informed changes, and learn from their effects. Drawing on existing knowledge is a method it uses to find suitable design approaches. Revisions to the skill use the same process, starting from a need observed in a design conversation.

## How the steps fit together

The **vision** establishes the purpose and what success would mean. The **functional architecture** describes the responsibilities and interactions that could fulfill that purpose in technology-independent terms. The **design approach** draws on existing knowledge to find ways of organizing that work. **Technology selection** identifies tools that support the approach. **Implementation** makes the design concrete at the depth needed for the current decision.

At each step, consider both ordinary use and a plausible future change. Evidence can send the conversation back to any affected decision. For a small system, a brief conversation may be enough. Greater uncertainty can warrant more investigation.

Use `be-more-pedagogical` when available. Apply its principles to how you formulate the problem and assess the recommendation as well as how you explain them to the user. Start with why the stage matters, connect the explanation step by step, define unfamiliar terms, and distinguish evidence from assumptions. Use a concrete example when it helps explain the recommendation. Compare the proposed result with the goal and check for gaps before advancing. Match the depth to the user's knowledge and the decision at hand.

Start with the decision the user faces. Work through a concrete case together. Offer a provisional interpretation they can correct, and ask the question whose answer would most change the design. Use the stages below as moves in a conversation. Enter wherever the user already has evidence and return to earlier choices when an assumption changes. Let the user decide when a sketch, decision note, or other artifact would help.

## Design for continuing change

Treat the ability to evolve as part of the system's purpose and design. Throughout the conversation, consider how a person or agent can express a changed need, understand its implications, decide and carry out a change, and learn from its effects. Scale the supporting practices and capabilities to the system and the people involved.

When a need or observation changes, find the earliest design assumption it challenges. Revisit that assumption with the user, then follow its consequences through the functions, approaches, technologies, and implementation that depend on it. Carry forward decisions whose reasoning still holds. Use a concrete case to judge the revised design, and identify what subsequent use would tell you about it. Apply this rule to the process used to evolve the system as well.

## 1. Establish the vision

Ask who needs what to change and why it matters. Walk through an occasion when that person would use the system. What happens today? What would they be able to do differently? Who else experiences the consequences? Use their answers to locate the boundary of the undertaking and recognize success in practice. Keep candidate products out of the vision. If a technology is already mandated, carry it forward as a constraint.

Walk through a plausible future change as well. Who would express the new need, what would they need to understand, and how would they recognize a successful change? Include this capacity to evolve in the vision. Establish which decisions people want to make themselves and where they want assistance or automation.

## 2. Define the functional architecture

Follow the same case from trigger to outcome. Name each essential responsibility in domain language, such as “recognize an eligible request” or “resolve competing claims.” Locate who has authority, what knowledge passes between responsibilities, and what happens when a usual assumption fails. A responsibility may belong to a person, an agent, software, or an existing institution. Leave that allocation open when it has no bearing on the decision.

Follow the future change from the expressed need through understanding, decision, implementation, and observation. Locate who or what carries each responsibility and how those responsibilities connect to the system's ordinary operation. Ask how its purpose, rules, and design decisions remain available and consistent with what it actually does. Work out how a change reaches affected parts and existing users or information.

Try a second case where the boundary is uncertain. Split or combine responsibilities if doing so explains a real difference in behavior or ownership. Stop when you and the user can reason about the important choices.

## 3. Find the design approach

Ask together: *What do we already know about problems like this that could shape how we design the system?* Apply the three moves below to the important challenges in operating and evolving it.

1. **Recognize the underlying challenge.** Pick a case from the functional architecture and name the difficulty in the user's terms. For example, two teams classify the same request differently, and that changes who can act on it.
2. **Draw on existing knowledge.** Look for theories, methods, or working systems that address that difficulty, including in other fields. Bring back the idea worth borrowing and an example of where it has been used. In the classification case, a shared glossary and a formal ontology are both candidates.
3. **Judge what belongs in this design.** With the user, ask what each idea would change in the original case. A glossary might let the teams settle disagreements. An ontology might guide the designers, or the system might use it to interpret requests. Choose an approach, or combine several when each serves a distinct purpose. Be able to say why each belongs. Choose tools in the next step.

## 4. Choose technology to fit the approach

Before naming tools, ask what someone needs to be able to do in a concrete case and which constraints matter. Use those answers to find plausible options. Include what the team already uses when it could meet the need.

Compare the options on that same case. Check the capabilities that would decide the choice against current documentation or evidence from comparable use. Explain the tradeoff that matters to the user and what would make you reconsider. Leave the choice open if it can wait.

Walk the future change through the proposed tools too. Check how people or agents would understand the current system, coordinate the affected changes, and observe the result. Let difficulties in that walkthrough inform the choice.

## 5. Enter implementation when it helps decide or build

Stay at the user's chosen depth. When a major choice rests on feasibility, suggest the smallest walkthrough or experiment that could distinguish the options. Move into implementation details when the user wants to build or when a particular detail could overturn the design. Return what was learned to the relevant earlier decision.

When implementing an evolution capability, try a small representative change through it. Check that the resulting behavior and the maintained understanding agree, and that existing users and information make the transition as intended. Use that experience to refine how future changes will work.

## Close the feedback loop on every pass

While considering a change, name the outcome you expect and how someone could observe it. Use a real case, a conversation, or an existing signal when possible. Agree who can interpret the evidence, when it warrants attention, and who can decide to keep, revise, or retire the change. After acting, compare the next observation with the expectation. Look for effects on people beyond the immediate user.

Ask whether the feedback concerns the system's behavior or the way changes are understood and carried out, or both. Follow the affected assumptions using the rule above. Where others will need to pick up the work, use their existing medium to retain the decision, its reason, and what would reopen it.

Use the same discipline when changing this skill. Trace a correction to the instruction that shaped the decision, try the smallest useful revision, and revisit its effect on a subsequent case. End the current pass when the decision is clear enough to act on or the next observation depends on real use.

## Ideas this builds on

- **Systems engineering** connects stakeholder needs, requirements, functions, and alternative designs through an iterative process. This skill adapts stakeholder scenarios and logical decomposition to its vision and functional architecture steps. [NASA Systems Engineering Handbook, §4](https://www.nasa.gov/reference/4-0-system-design-processes/)
- **Enabling systems** support a product through its life, including development and maintenance. Considering the product and those supporting systems together provides a basis for designing how it will evolve. [Systems Engineering Body of Knowledge](https://sebokwiki.org/wiki/Product_as_a_System_Fundamentals)
- **The Model for Improvement** connects an aim, evidence of improvement, and changes to try through Plan–Do–Study–Act cycles. It informs the skill's practice of comparing the effects of a change with what was expected. [Institute for Healthcare Improvement](https://www.ihi.org/library/model-for-improvement)

The five-step arrangement and its use in a person–agent conversation are this skill's synthesis of these ideas. Its usefulness is being refined through use. The references explain its foundations; choose design methods for each system through step 3.
