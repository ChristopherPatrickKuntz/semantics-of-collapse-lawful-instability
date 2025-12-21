# Glossary

## Agent

Any automated utility-maximizing actor. Includes AI systems, MEV bots, algorithmic trading systems, smart contract automations, and autonomous infrastructure controllers.

The defining characteristic is not sentience but optimization: agents act to maximize a utility function faster than human reaction time permits intervention.

## Lawful Instability

A failure mode in which systems collapse while all actions remain valid, authorized, and policy-compliant.

Lawful instability is the parent taxonomy. Specific manifestations include hysteresis exploitation, state-entropy expansion, and incentive inversion.

## Validity-Safety Orthogonality Problem

The observation that validity (conforming to rules) and safety (preserving system integrity) are orthogonal rather than correlated.

Traditional security frameworks implicitly assume these are correlated. Agentic systems violate this assumption.

## Safe-to-Exist Analysis (SEA)

A complementary security primitive that uses conservation-based global invariants to constrain system behavior.

Rather than validating individual actions, SEA defines properties that must be preserved across all state transitions.

## Global Invariant

A property that must remain true (or bounded) across all possible sequences of valid operations.

Examples: total value conservation, liquidity ratio bounds, state entropy limits.

## Conservation-Based Invariant

An invariant modeled on physical conservation laws. Defines a quantity that cannot be created or destroyed, only transferred or transformed within bounds.

## Hysteresis Exploitation

Exploiting the temporal lag between state observation and state reconciliation.

Example: Liquidity vampire attacks that withdraw liquidity before large trades and re-deposit after.

## State-Entropy Expansion

Exploiting the asymmetric cost of write operations vs. persistent storage and indexing.

Example: Computational dust attacks that create minimal-balance accounts to bloat system state.

## Incentive Inversion

Exploiting reward systems designed for negative feedback loops.

Example: Creating problems to earn rewards for solving them.

## Phase Margin Erosion

A control theory concept. Agents operating at computational speed can destabilize feedback loops by eroding the phase margin of the system's transfer function.

Systems designed for human-latency interaction become unstable when subjected to agent-latency control inputs.
