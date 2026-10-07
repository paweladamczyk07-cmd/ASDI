# ASDI

ASDI extends Proto-ASDI from model-building toward an agent capable of directing more of its own development.

The defining shift is:

Proto-ASDI: I can build and revise models.

ASDI: I can use those models to decide what I need to learn next, how to test it, and how to improve my own learning process.

## Conceptual architecture

1. Perception - what is observed.
2. Memory - what has been experienced.
3. Knowledge/Doubt - what is supported and what remains uncertain.
4. World model - hypotheses about relationships and causes.
5. Prediction - possible future states.
6. Action - interaction with the environment.
7. Experiment selection - choosing actions for information as well as outcome.
8. Observer/Curiosity - identifying valuable uncertainty.
9. Self-evaluation - measuring prediction quality and learning efficiency.
10. Learning-process adaptation - changing how the agent allocates attention, experiments, memory, or model-building effort.

## A deeper loop

observe -> hypothesize -> predict -> choose action/experiment -> observe consequence -> compare prediction with reality -> update knowledge and doubt -> revise model -> evaluate learning efficiency -> choose what to learn next.

The final step is important. The agent is no longer merely learning about the environment; it is beginning to learn about how it learns.

## Inductive and deductive processes

Induction: observations generate candidate rules or models.

Deduction: a model generates predictions that can be checked against observations.

A mature loop therefore becomes:

observation -> induction -> model -> deduction -> prediction -> experiment -> observation.

Neither direction is sufficient by itself.

## Counterfactual reasoning

Once a causal model exists, the agent can ask questions about states that have not actually occurred:

- What would happen if I did something else?
- Which observation would distinguish these two explanations?
- Which experiment is safest or cheapest?
- What evidence would prove this model wrong?

This is more powerful than memorizing successful responses.

## Self-development

ASDI treats development as an object of optimization.

The system can potentially evaluate which memories are useful, which uncertainties matter, which models generalize, which experiments produce information, which learning strategies waste resources, and when to stop exploring.

This does not require unrestricted self-modification. The initial concept can remain bounded, inspectable, and externally evaluated.

## Scope

ASDI is a hypothesis about a class of cognitive architectures. It is not a claim that present-day AI already implements this architecture, nor a claim about consciousness or subjective experience.
