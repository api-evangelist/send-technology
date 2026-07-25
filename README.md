# Send Technology (send-technology)

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
