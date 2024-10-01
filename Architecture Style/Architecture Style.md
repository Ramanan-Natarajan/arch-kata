## Architectural Style

**Application:** Clear View

**Date:**  30-09-2024
-
**Sta0tus:** Proposed

**Deciders:** Clear View Engineering Team

**Context:**

We are designing the architecture for Clear View, a service-oriented application that requires high degrees of deployability, evolvability, interoperability, and efficient workflow management. This necessitates an architecture that enables independent deployments, seamless updates, technology diversity, and effective orchestration of complex interactions between services.

**Decision:**

- We will adopt a microservices based architecture with clear service boundaries and contracts as the core architectural style. 
- We will use Asynchronous eventing wherever required. 
- We will favour orchestration over choreography when orchestrating multiple microservices, as we have complex workflows, and a clear error handling is easy in this approach. It also eases the engineer cognitive load and lends itself to simple reasoning



**Consequences:**

* **Positive:**
    * **Enhanced Deployability:**  Independent deployments of Clear View services with minimal downtime and reduced risk.
    * **Improved Evolvability:**  Seamless updates and modifications of individual services without impacting others.
    * **Increased Interoperability:** Flexibility to use diverse technologies for different Clear View services while maintaining seamless communication.
    * **Efficient Workflow Management:**  Orchestration of complex business processes through event-driven workflows.
    * **Improved Resilience and Fault Tolerance:**  Isolation of services minimizes the impact of failures and enhances system stability.

* **Negative:**
    * **Debugging Challenges:**  Tracing events and identifying root causes of issues can be more challenging compared to synchronous communication.
  


**Notes:**

This ADR will be reviewed and updated as the Clear View project progresses and new insights emerge.

Architecture Characteristic Worksheet<img src="../diagrams/arch-char.jpg">
