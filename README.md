# The Art of Agentic Development

This space contains my thoughts, opinions, and learnings when building production grade agent-enabled systems and workflows.

## Definitions

We define an agent as an instructed large language model. An instruction here typically would consist of:
- A role definition—a perspective you are taking as the agent
- A set of clear instructions for what to do
- A definition of what input is expected to be given (e.g., size of screen, image, fields, properties, types of data)
- Clear output expectations (could be a template file content or instructions as to how to format, postprocess, and serve the output)

We define an agentic system as a system that needs to make some sort of decision, whether it is interpreting information or data, or triggering other systems or the agents. To some degree, in some cases, it will also be for systems that are meant to learn as they go and self-improve. Although it is very few places in today's industry where this is even being attempted in the sense that automnomous operation is possible at higher level than simple workflows or compacted processes (OpenAI, Google, Meta, Microsoft, Anthropic, and these kinds of companies).

First, we declare two points:
1. We want to have agentic systems that are inherently deterministic.
2. We differ between deterministic automation and non-deterministic automation when building agentic systems.

## The Sweet Spot

Currently, agentic systems are not good enough to be working on the entire process end-to-end and making all decisions by themselves. Instead, the most stable production agentic solutions one can achieve at the moment will be systems that are predominantly deterministic by design, where you use agents (instructed LLMs) for the portions that are not easily automatable by code. 
