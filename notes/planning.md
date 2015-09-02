Planning is tricky because:

- environmental properties:
    - systems may be _stochastic_
    - there may be _multiple agents_ in the system
    - there may be _partial observability_ (that is, the state of the system may not be fully known)
- agent properties:
    - some information may be _unknown_
    - plans are hierarchical (high level to low level parts)

In planning we represent the world in _belief states_, in which multiple states are possible (because of incomplete information, we are not certain what the true state of the world is). Actions that are taken can either increase or decrease the possible states, in some cases down to one state.

Sequences of actions can be defined as trees, where each branch is an action and each node is a state or is an observation of the world. Then we search this tree for a plan which will satisfy the goal.