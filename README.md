# Send Technology (send-technology)

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

Send Technology Solutions Ltd is a London-headquartered insurtech software company, founded in 2017, that builds an underwriting workbench for commercial and specialty insurers, MGAs and reinsurers. Its platform covers submission management, quote and rate lifecycle management, risk workflow, binder management, bordereaux ingestion, entity management, post-bind processing and portfolio data and insights, with product lines for direct underwriting, delegated underwriting and reinsurance underwriting. Its home market is the United Kingdom and its centre of gravity is the London Market — Lloyd's managing agents, syndicates and MGAs — where it ships pre-built connectors to the electronic placing platforms PPL and Whitespace and aligns with Lloyd's Blueprint Two.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/send-technology/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/send-technology/refs/heads/main/apis.yml)

## Tags

- Insurance
- United Kingdom
- Insurtech
- Underwriting
- London Market
- Lloyd's of London
- Specialty Insurance
- Commercial Insurance
- Reinsurance
- Delegated Authority
- MGA
- Policy Administration
- ACORD
- Partner Gated

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

**None listed — no public API.**

Send markets itself as "an API-first platform with pre-built connectors for placing platforms like Whitespace and PPL, insurance-focused data integrations, rating engines, document stores, and policy admin systems," but it publishes no public developer portal, no API reference, and no downloadable API definition.

Probed on 2026-07-25:

| Candidate | Result |
| --- | --- |
| `developer.send.technology` | DNS does not resolve |
| `developers.send.technology` | DNS does not resolve |
| `docs.send.technology` | DNS does not resolve |
| `api.send.technology` | DNS does not resolve |
| `send.technology/developers` | 404 |
| `send.technology/developer` | 404 |
| `send.technology/api` | 404 |
| `send.technology/integrations` | 404 |
| `send.technology/openapi.json`, `/swagger.json`, `/api-docs`, `/spec`, `/redoc`, `/v1/openapi.json` | 404 |
| `send.technology/graphql` | 404 |
| `send.technology/.well-known/openid-configuration` | 404 |
| [send.technology/partners](https://send.technology/partners/) | 200 — marketing partner directory, not a developer portal |

The full public page sitemap (43 pages) contains no developer-, docs- or API-facing page. There is no `github.com/send-technology` organization, no public Postman workspace, no GraphQL surface, no published `.proto`, and no webhook or AsyncAPI event catalog. Zero OpenAPI/Swagger definitions were harvested, and the `openapi/` directory is intentionally absent.

The only integration surface is partner- and customer-gated: connectors are configured during a commercial implementation, and standards-based exchange runs through ACORD Solutions Group rather than through anything a developer can sign up for.

## ACORD Posture

**ACORD member; ACORD Standard placing/accounting/claims transactions exchanged via ACORD Solutions Group's ADEPT API; ACORD Forms ingestion for submission triage.**

Send announced a strategic partnership with ACORD Solutions Group, the digital solutions subsidiary of ACORD, and uses ADEPT (ACORD Data Exchange Platform and Translator) via API so that Send customers can send and receive ACORD Standard accounting, claims and placing transactions — eMessaging aligned with Lloyd's Blueprint Two. Send is also an ACORD member and ingests ACORD Forms to classify and triage new submissions. No AL3 flat-file reference and no IVANS / Applied Epic / Vertafore AMS360 agency-download reference was found, which is consistent with a London Market rather than a US agency-management footprint.

## Quote / Bind / Issue / FNOL

All of quote, bind and issue are covered by the *product* — Quote & Rate Lifecycle Management, Send Rating, Send Studio, Binder Management, Post-Bind Processing — but none of them is exposed as a public API. FNOL is not a Send product area; claims appear only as ACORD claims transactions carried over ADEPT. The audience is partner-only: licensed underwriters, managing agents, MGAs and reinsurers.

## Platform Modules

- Submission Management (Send Flow)
- Quote & Rate Lifecycle Management (Send Rating, Send Studio)
- Risk Workflow
- Automation & Rules
- Activity Management
- Binder Management
- Bordereaux Ingestion
- Entity Management
- Post-Bind Processing
- Data & Insights
- Agentic Framework (managed, partner and custom agents over AWS Bedrock, Azure and OpenAI, under ISO 42001)

## Links

- [Website](https://send.technology/)
- [About](https://send.technology/about/)
- [Platform](https://send.technology/platform/)
- [Partners](https://send.technology/partners/)
- [London Market solution](https://send.technology/solutions/london-market/)
- [Agentic Framework](https://send.technology/agentic-framework/)
- [Blog](https://send.technology/resources/blog/)
- [Blog RSS](https://send.technology/resources/blog/feed/)
- [LinkedIn](https://www.linkedin.com/company/send-technology-solutions)
