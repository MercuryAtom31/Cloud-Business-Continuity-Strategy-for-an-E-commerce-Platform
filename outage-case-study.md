# Outage Case Study: Cloud Service Disruption and E-commerce Continuity

## Purpose
This case study examines a realistic cloud outage scenario affecting a modern e-commerce platform. It shows how dependency failures can disrupt customer transactions, what response actions are most effective, and which continuity improvements should be prioritized.

## Scenario Overview
The company runs its storefront and APIs on a managed cloud application platform with DNS and edge protection from a cloud network provider. It also relies on:

- A third-party identity provider for sign-in and account sessions.
- A third-party payment processor for checkout authorization.

During a high-traffic sales event, a regional cloud networking and platform incident causes elevated latency, intermittent API errors, and request timeouts.

## Business Context

- Traffic was approximately 2.4x normal weekday baseline.
- Promotion campaign was active across email and social channels.
- Checkout abandonment sensitivity was high due to price-driven customers.

The organization had monitoring and alerting in place, but not all dependency health checks were tied to automated failover decisions.
