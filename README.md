# AiDASH

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
