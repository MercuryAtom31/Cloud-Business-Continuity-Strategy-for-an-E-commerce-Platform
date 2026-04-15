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

## Incident Timeline

### T+00 minutes
Synthetic monitors detect increased error rates on API endpoints.

### T+05 minutes
Customer support reports that users can browse products but fail at login and checkout intermittently.

### T+10 minutes
On-call engineer confirms platform-level latency and dependency timeouts. Incident severity is escalated.

### T+15 minutes
Incident manager activates continuity workflow and starts stakeholder communication cadence.

### T+20 minutes
Traffic steering to secondary environment begins for read-heavy storefront routes.

### T+30 minutes
Login failures continue because identity service in the primary path remains unstable.

### T+40 minutes
Guest checkout fallback is enabled for eligible users.

### T+50 minutes
Payment retries are queued with user-facing messaging instead of hard transaction failure.

### T+70 minutes
Primary region begins recovering, but elevated latency persists.

### T+90 minutes
Core browsing and checkout stabilize, though account features remain partially degraded.

### T+120 minutes
Incident status moved from active response to monitored recovery.

## Observed Customer Impact

- Users experienced intermittent login and checkout failures.
- Average page response time increased significantly during the first 45 minutes.
- Conversion rate dropped during peak incident window.
- Cart abandonment increased due to repeated payment failures and session interruptions.

## Operational Impact

- Support ticket volume spiked.
- Incident response consumed engineering and operations capacity for several hours.
- Marketing campaign efficiency declined because paid traffic reached partially degraded services.

## Root Cause Summary
The immediate trigger was a regional cloud service disruption affecting network and managed application platform stability. The largest business impact came from dependency coupling:

- Authentication path had no fast temporary bypass for account-required flows.
- Payment retry strategy existed but was not fully automated at incident start.
- Failover focused first on browsing availability and did not initially preserve all checkout dependencies.

No evidence indicated data corruption, but transaction completion was degraded for a significant portion of customers.

## Response What Worked Well

- Early detection from synthetic monitoring reduced time to incident declaration.
- Incident manager role was activated quickly.
- Customer-facing status updates were published at regular intervals.
- Guest checkout fallback reduced total lost sales after activation.
- Read-path failover protected product browsing and search for most users.
