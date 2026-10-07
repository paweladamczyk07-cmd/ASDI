# Proto-ASDI

Proto-ASDI describes an early architecture for an agent that can move beyond simple consequence-driven adaptation.

## The central loop

Observe -> represent -> predict -> act -> compare -> revise.

The agent does not only store that an action succeeded or failed. It attempts to retain a representation of why the result occurred.

A conceptual state contains:

- Observation
- Context
- Current model
- Prediction
- Action
- Consequence
- Prediction error
- Confidence
- Revised model

## From reward to information

Traditional reinforcement learning can ask: Which action gives the highest reward?

Proto-ASDI adds: Which action would teach me something important?

An action can therefore have two values:

1. Outcome value - how desirable the consequence is.
2. Information value - how much the consequence can improve or discriminate the agent's model.

This permits deliberate exploration rather than exploration being only noise around exploitation.

## Knowledge and Doubt

Proto-ASDI explicitly separates:

Knowledge - this model currently has strong support.

Doubt - there is evidence that this model may be incomplete, wrong, or applicable only in some contexts.

Doubt is not failure. It is a navigational signal for further observation or experiment.

## Fact and Fiction

The agent should distinguish observed or internally validated information from hypothetical constructions.

A hypothetical model may be useful while remaining marked as hypothetical.

This permits:

fact -> hypothesis -> prediction -> experiment -> evidence -> updated fact/model.

## Curiosity and the Observer

A conceptual observer can monitor unexplained prediction errors, persistent uncertainty, novel states, conflicts between models, and opportunities for informative experiments.

The observer does not need to know the answer. Its function is to identify where learning is valuable.

## Locality and memory

The early grid-world formulation used limited local observation and limited memory. The environment could grow beyond the agent's immediate view.

This matters because an agent must eventually learn that the visible state is not the whole environment, unseen structure can be inferred, memory changes what can be predicted, and exploration changes the information available later.

## Stopping condition

Learning should not continue indefinitely merely because learning is possible.

A useful conceptual rule is:

continue learning while expected useful information > learning cost.

This makes curiosity selective rather than compulsive.

## Proto-ASDI is not AGI

Proto-ASDI is a proposed architectural direction. It does not imply consciousness, human-level intelligence, or unrestricted autonomy.

Its purpose is narrower: give an adaptive agent machinery to build, test, doubt, and revise models of its environment.
