# ADR-004: Leveraging and Abstracting Large Language Models (LLMs)

### Date: 2024-09-30

### Status: Accepted

### Decision Maker: Engineering Team

### Context:

Our Clearview application aims to provide features like resume pre-screening, resume building, refinement and resume story generation. Large Language Models (LLMs) offer powerful capabilities for natural language processing and understanding, making them well-suited for these tasks.

### Decision:

We will assume that we are provided a well trained, grounded LLM as a core component of our application.

To avoid vendor lock-in and maintain flexibility, we will abstract the LLM integration behind a well-defined interface. This abstraction layer will enable us to:

- Plug in multiple LLMs: We can easily switch between different LLM providers (e.g., OpenAI, Google AI, Cohere) without significant code changes.
- A/B test different LLMs: We can compare the performance and effectiveness of different LLMs in a controlled environment to identify the best option for our needs.
- Adapt to future advancements: The abstraction layer will allow us to seamlessly upgrade to newer and more capable LLMs as they become available.


### Consequences:

**Enhanced functionality**: LLMs will enable us to provide advanced features like accurate resume pre-screening, insightful resume story generation, and personalized candidate recommendations to job fitments.
**Increased flexibility**: The abstraction layer will allow us to adapt to the evolving LLM landscape and leverage the best available technology.
**Potential ethical considerations**: We will need to carefully consider the ethical implications of using LLMs, especially in the context of sensitive HR data (Personally identifiable information data). We will assume that the model will not exhibit bias

### Assumptions:

A suitable trained, grounded LLM is available today that meets our performance and accuracy requirements.


### Notes:

This ADR establishes our intention to leverage the power of LLMs while maintaining flexibility and control over our technology stack.