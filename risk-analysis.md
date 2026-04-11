# Risk Analysis for the E-commerce Platform

## Purpose
This document identifies the main risks that could disrupt the cloud-based e-commerce platform and evaluates their business impact, likelihood, and mitigation options. The analysis is focused on business continuity rather than on purely technical failure modes.

## Risk Rating Method
Each risk is rated using a simple scale:

- Likelihood: Low, Medium, High
- Impact: Low, Medium, High

Risks with high likelihood and high impact require the fastest and most complete mitigation.

## Summary of Major Risks

| Risk | Likelihood | Impact | Business Effect |
| --- | --- | --- | --- |
| Cloud platform outage | Medium | High | Storefront and API unavailable |
| Regional service failure | Medium | High | Partial or total loss of service in one region |
| DNS or edge protection failure | Low | High | Customers cannot reach the site |
| Identity provider outage | Medium | High | Users cannot sign in or complete account actions |
| Payment processor outage | Medium | High | Checkout is interrupted and revenue is lost |
| Data corruption or data loss | Low | High | Orders or customer records may be damaged |
| Cyberattack or account compromise | Medium | High | Service interruption, data exposure, or fraud |
| Capacity or scaling failure | Medium | Medium | Slow performance and abandoned carts |
| Human error in configuration changes | High | Medium | Service instability or outage during deployment |
| Third-party dependency failure | Medium | High | Downstream business services become unavailable |
