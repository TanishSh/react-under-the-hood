# ReAct Under the Hood

## Research Question

Does explicitly interleaving reasoning traces with environment interactions
improve the reliability of a modern open-weight language model on multi-hop
question answering?

## Conditions

We compare:

1. Direct Answer
2. Tool-Only Agent
3. ReAct Agent

All conditions use:
- the same language model
- the same HotpotQA evaluation examples
- the same decoding settings
- the same maximum answer budget

Tool-Only and ReAct additionally receive the same Wikipedia interface.

## Primary Hypothesis

ReAct will outperform direct answering because the model can retrieve missing
information and reason over intermediate observations.

## Ablation Hypothesis

ReAct will outperform Tool-Only because explicit reasoning traces help the
model decide what information to retrieve and how to combine observations.

## Secondary Research Question

What types of failures remain after adding ReAct?