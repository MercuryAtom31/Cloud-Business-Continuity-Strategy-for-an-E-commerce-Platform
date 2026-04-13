# Outage Case Study: Cloud Service Disruption and E-commerce Continuity

## Purpose
This case study examines a realistic cloud outage scenario affecting a modern e-commerce platform. It shows how dependency failures can disrupt customer transactions, what response actions are most effective, and which continuity improvements should be prioritized.

## Scenario Overview
The company runs its storefront and APIs on a managed cloud application platform with DNS and edge protection from a cloud network provider. It also relies on:

- A third-party identity provider for sign-in and account sessions.
- A third-party payment processor for checkout authorization.

During a high-traffic sales event, a regional cloud networking and platform incident causes elevated latency, intermittent API errors, and request timeouts.
