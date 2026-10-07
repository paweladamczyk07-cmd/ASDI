# ASDI - Conceptual Map

ASDI is a working name for a family of architectures concerned with self-development through interaction with an environment.

The project is a conceptual research notebook, not a finished implementation.

## Lineage

Dual-core agent -> reward discovery -> curiosity/observation -> internal knowledge and doubt -> model building -> autonomous experimentation -> self-development.

The early dual-core idea separates acting from evaluating. A later observer/curiosity component asks what is unknown and what information is worth obtaining.

## Important components

### Observation
The agent distinguishes what it directly observes from what it infers.

### Knowledge
Representations supported by repeated or otherwise validated observations.

### Doubt
Explicit uncertainty about whether a representation is correct.

### Model
A structured hypothesis about how observations, actions, and consequences relate.

### Prediction
Using the model to estimate possible future states before acting.

### Experiment
Selecting an action partly because its result can distinguish between competing hypotheses.

### Curiosity
A drive toward reducing useful uncertainty rather than merely maximizing an externally supplied reward.

### Memory
Retention of observations, consequences, models, failed predictions, and useful distinctions.

### Self-correction
Revision of internal representations when prediction and observation disagree.

## Design principle

The key transition is from:

What response worked here?

to:

What kind of environment produces this result?

That transition is the conceptual heart of Proto-ASDI.

## What this does not claim

This repository does not claim that such an architecture is conscious, sentient, alive, or morally equivalent to a person. It describes mechanisms and hypotheses that can be discussed and tested.
