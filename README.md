# Cloud Business Continuity Case Study for an Online Retail Platform

## Overview
This repository presents a business continuity case study for a cloud-based online retail platform. The objective is to assess how Infrastructure as a Service (IaaS) and Platform as a Service (PaaS) affect business continuity planning, analyze real cloud outage lessons, and define response, recovery, and continuity testing activities.

The scenario assumes a modern online business with:
- DNS and edge protection provided by a cloud network provider
- Frontend, backend, and database hosted on a managed cloud application platform
- Online payments handled by a third-party payment processor
- Authentication handled by a third-party identity provider

## Essential Questions
1. How do IaaS and PaaS impact business continuity planning?
2. Have cloud providers experienced major outages that affect customers?
3. If an organization uses cloud providers for continuity services, what response, recovery, and continuity testing should it conduct?

## What this repository contains
- A written assessment
- A cloud continuity architecture diagram
- A response and recovery workflow diagram
- A testing plan
- A source list

## Current Deliverables
- Business continuity strategy: [bcp-strategy.md](bcp-strategy.md)
- Risk analysis: [risk-analysis.md](risk-analysis.md)
- Outage case study: [outage-case-study.md](outage-case-study.md)
- Cloud continuity architecture diagram: [cloud-continuity-architecture-diagram.puml](cloud-continuity-architecture-diagram.puml)
- Response and recovery workflow diagram: [response-recovery-workflow.puml](response-recovery-workflow.puml)
- Testing plan: [testing-plan.md](testing-plan.md)
- Source list: [sources.md](sources.md)

## Key Takeaways
- Cloud improves resilience, but it does not remove continuity risk.
- Vendor outages, IAM failures, and third-party dependencies must be part of business continuity planning.
- Response, recovery, and testing must include both the organization’s own systems and its external service providers.
