# Abstract

Contemporary security frameworks (OWASP, NIST CSF, MITRE ATT&CK) share a common ontological assumption: security failures result from deviation from specified behavior. These frameworks excel at detecting aberrations - unauthorized access, malformed inputs, violated policies.

However, the emergence of autonomous economic agents introduces a categorically different threat model: systemic instability through strict adherence to permitted behavior. When rational optimizers interact with systems at computational speed, they exploit not vulnerabilities in the traditional sense, but rather gradient surfaces in business logic - mathematical structures that incentivize behaviors which are individually valid yet collectively catastrophic.

**Central Thesis:** Current security paradigms systematically fail to model threats where:

1. All state transitions are valid regarding the schema
2. All authentication and authorization checks pass
3. All rate limits are respected
4. All monitoring dashboards remain "green" until the moment of collapse

This is termed the **Validity-Safety Orthogonality Problem** - a specific manifestation of Lawful Instability.

This paper formalizes this blind spot using established theory from control systems and distributed computing, then proposes conservation-based invariants as a mandatory complementary security primitive.

**Core Argument:** For an agentic system, lawful instability is the default state unless explicitly constrained by global invariants.

---

## Terminology

Throughout this paper, "agent" refers to any automated utility-maximizing actor - including but not limited to AI systems, MEV bots, algorithmic trading systems, smart contract automations, and autonomous infrastructure controllers.

The defining characteristic is not sentience but optimization: agents act to maximize a utility function faster than human reaction time permits intervention.
