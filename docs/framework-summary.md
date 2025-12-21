# Safe-to-Exist Analysis (SEA) Framework Summary

## The Problem SEA Addresses

Traditional security tools map to the left half of the validity-safety matrix (invalid actions). Modern security research focuses on moving attacks from "undetected" to "detected" within the Invalid column.

SEA addresses the right half - where detection is irrelevant because the actions are legitimate.

## Core Insight

You cannot "patch" your way out of lawful instability. The vulnerability is not in the code. It is in the game theory.

## The SEA Approach

SEA proposes conservation-based invariants as the primary defense against lawful instability.

Rather than validating individual actions, SEA defines global properties that must be preserved across all state transitions, regardless of how valid those transitions are individually.

### Conservation Invariants

A conservation invariant defines a quantity or relationship that must remain stable (or bounded) across time, independent of the sequence of valid operations.

Examples:

- **Total value conservation**: The sum of all assets in the system cannot increase without external deposits
- **Liquidity ratio bounds**: The ratio of available liquidity to outstanding obligations must remain above a threshold
- **Entropy bounds**: The state entropy of the system cannot grow faster than a specified rate

### Why Conservation Works

Conservation-based invariants operate at a different abstraction layer than action validation:

| Layer | Traditional Security | SEA |
|-------|---------------------|-----|
| Focus | Individual actions | Global state properties |
| Question | "Is this action permitted?" | "Does the system remain stable?" |
| Failure mode | Unauthorized action | Authorized but destabilizing action |
| Defense | Access control, validation | Invariant enforcement |

## Historical Precedent

Conservation invariants are not novel in complex systems:

- **Financial markets**: Circuit breakers halt trading during extreme moves (price conservation bounds)
- **Physics**: Conservation of energy, momentum, charge
- **Database systems**: ACID properties, referential integrity
- **Distributed systems**: Consistency models, quorum requirements

SEA extends this principle to agentic system security explicitly.

## Application

For any system with autonomous optimizers:

1. Identify the global properties that define "system health"
2. Formalize these as conservation invariants
3. Enforce invariants at the protocol level, not the action level
4. Actions that would violate invariants are rejected regardless of their individual validity

This shifts the security question from "Did the user have permission?" to "Does the system remain stable?"
