# Relationship to Other Work

## Position Within Broader Research

This paper builds on and complements prior work on observability and security boundaries in agentic systems.

### The Pre-Articulation Observability Boundary

Prior work identifies structural limits on language-based system interpretation - what systems cannot observe about user intent before it is explicitly articulated.

### This Paper: The Stability Boundary

This work identifies structural limits on what systems can safely permit - even when all actions are valid and observable.

## Orthogonal Components

Together, these works define:

- **An observability boundary**: What systems cannot see
- **A stability boundary**: What systems cannot safely allow

They are intended as orthogonal components of a broader agentic systems security framework.

## Relationship to Existing Security Frameworks

| Framework | Focus | Blind Spot Addressed by SEA |
|-----------|-------|----------------------------|
| OWASP | Web application vulnerabilities | Valid actions that destabilize |
| NIST CSF | Risk management process | Risks from permitted behavior |
| MITRE ATT&CK | Adversary tactics and techniques | Tactics using only authorized actions |
| CVE/NVD | Known vulnerabilities | Emergent risks with no CVE |

SEA does not replace these frameworks. It addresses a complementary failure class they are structurally unable to model.

## Theoretical Foundations

This work synthesizes established theory from multiple fields:

- **Control Theory**: Nyquist stability criterion, phase margin analysis
- **Distributed Systems**: CAP theorem, consistency models
- **Algorithmic Game Theory**: Mechanism design, equilibrium analysis
- **Complex Systems**: Reflexivity, feedback instability

The contribution is not new theory in any single field, but the synthesis and application to agentic system security.
