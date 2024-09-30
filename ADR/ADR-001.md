# ADR-001: Primacy of ADRs

### Date: 2024-09-30

### Status: Accepted

### Decision Maker: Engineering team

### Context:

We need a mechanism to ensure that architecturally significant decisions are made deliberately, transparently, and with their impact's understood. This will help us to:

- Maintain a consistent architectural vision and avoid achitectural divergence
- Avoid costly rework due to inconsistent or poorly-considered decisions. Will help us look at the second right answer and evaluate available options
- Onboard new team members more effectivel and Improve communication and collaboration within the team.
- Explain the **whys** more than the **how's**

### Decision:

All architecturally significant decisions will be discussed and documented as an Architectural Decision Record (ADR). An ADR is a short document that captures the following information:

**Title**: A clear, concise and descriptive title for the decision.
**Context**: The background and rationale for the decision.
**Decision**: The actual decision that was made.
**Consequences**: The potential implications of the decision.
**Status**: The current status of the decision (e.g., proposed, accepted, deprecated).

ADRs will be stored in the repo 

### Consequences:

- Increased transparency and accountability in architectural decision-making.
- Improved documentation of the system's architecture.
- A more consistent and maintainable architecture.
- Potentially increased overhead in the decision-making process.