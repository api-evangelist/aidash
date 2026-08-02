# AiDASH

AiDASH is an AI-first vertical SaaS company that uses satellite imagery and machine learning to run
operations, maintenance, and climate-resilience programs for industries with geographically distributed
assets — primarily electric and gas utilities, water companies, and landowners. Founded in 2019 and
headquartered in San Jose, California, with offices in the Washington D.C. metro area and Bengaluru.

- Website — https://www.aidash.com/
- Platform — https://www.aidash.com/platform/
- GitHub — https://github.com/aidash
- Trust Center — https://security.aidash.com/
- Status — https://aidash.statuspage.io/

## API surface

AiDASH markets "secure, full REST APIs" and industry-standard connectors on its platform page, but
publishes **no public developer portal, API reference, getting-started guide, or machine-readable
contract**. Contract discovery was run against every reachable host (`www.aidash.com`,
`iris.aidash.com`, `connect.aidash.com`, plus hosts discovered via DNS and certificate transparency)
for OpenAPI/Swagger, GraphQL introspection, MCP `tools/list`, and A2A agent cards — all missed. The
product API is customer-gated behind commercial engagement.

The one public, unauthenticated, machine-readable surface is the Atlassian Statuspage **Status API v2**
at `https://aidash.statuspage.io/api/v2`, covering the IVMS, RIMS, ISMS, and CRIS components.

## Artifacts

| Path | Type | Method |
|---|---|---|
| `llms/aidash-llms.txt` | LLMsTxt | searched (verbatim from `https://www.aidash.com/llms.txt`) |
| `lifecycle/aidash-lifecycle.yml` | Lifecycle + StatusPage | probed |
| `security/aidash-trust-center.yml` | TrustCenter | searched |
| `security/aidash-domain-security.yml` | DomainSecurity | probed |
| `conformance/aidash-conformance.yml` | Conformance | searched |
| `well-known/aidash-well-known.yml` | probe record (nothing published) | probed |

## Notes

- SOC 2 Type 2, a public SOC 3 report, and a CSA STAR Level 1 (CAIQ) self-assessment are published;
  no ISO 27001, HIPAA, PCI DSS, or FedRAMP.
- No `security.txt`, no published vulnerability-disclosure contact, and no bug-bounty program.
- No status subdomain (`status.aidash.com` does not resolve) — the status page lives at
  `aidash.statuspage.io`.
- In June 2026 Schneider Electric agreed to acquire ~90% of AiDASH at an implied enterprise value of
  USD 350 million, pending regulatory close.
