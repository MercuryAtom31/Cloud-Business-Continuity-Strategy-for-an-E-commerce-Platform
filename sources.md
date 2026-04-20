# Sources and References

## Purpose
This source list provides references used to support the business continuity strategy, risk analysis, outage case study, and continuity testing plan.

## Core Frameworks and Standards
1. National Institute of Standards and Technology (NIST), NIST SP 800-34 Rev. 1, *Contingency Planning Guide for Federal Information Systems*. Available at: https://csrc.nist.gov/publications/detail/sp/800-34/rev-1/final
2. ISO 22301, *Security and resilience - Business continuity management systems - Requirements*.
3. U.S. Cybersecurity and Infrastructure Security Agency (CISA), continuity and incident response guidance. Available at: https://www.cisa.gov

## Cloud Architecture and Resilience Guidance
1. Microsoft Azure Well-Architected Framework, Reliability pillar. Available at: https://learn.microsoft.com/azure/well-architected/reliability/
2. AWS Well-Architected Framework, Reliability pillar. Available at: https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/welcome.html
3. Google Cloud Architecture Framework, Reliability. Available at: https://cloud.google.com/architecture/framework/reliability

## Outage and Service Health References
1. Microsoft Azure Service Health status and incident communication. Available at: https://status.azure.com
2. AWS Service Health Dashboard and historical events. Available at: https://health.aws.amazon.com/health/status
3. Google Cloud Service Health dashboard. Available at: https://status.cloud.google.com
4. Cloudflare status and incident reports. Available at: https://www.cloudflarestatus.com

## Identity and Access Resilience References
1. Microsoft identity platform reliability and high availability guidance. Available at: https://learn.microsoft.com/entra/identity/
2. OAuth 2.0 and OpenID Connect specifications for identity flows:
   - OAuth 2.0 (RFC 6749): https://www.rfc-editor.org/rfc/rfc6749
   - OpenID Connect Core 1.0: https://openid.net/specs/openid-connect-core-1_0.html

## Payment and Transaction Reliability References
1. Stripe reliability and idempotency guidance. Available at: https://docs.stripe.com/idempotency
2. PCI Security Standards Council resources. Available at: https://www.pcisecuritystandards.org

## Incident Response and Communication
1. Google SRE Workbook, incident response and postmortems. Available at: https://sre.google/workbook/
2. Atlassian incident communication best practices (status communication patterns). Available at: https://www.atlassian.com/incident-management

## Notes on Source Usage
- Framework references support continuity structure, governance, and testing standards.
- Cloud status and outage references support outage-case assumptions and dependency risk discussion.
- Identity and payment references support dependency-specific continuity controls.
- Reliability and incident-response references support recovery workflow and communication practices.

## Citation Guidance for This Project
When citing within project documents, use a simple label style such as:
- [NIST-800-34]
- [Azure-Reliability]
- [Cloudflare-Status]
- [Stripe-Idempotency]

This keeps references clear and easy to trace back to this file.
