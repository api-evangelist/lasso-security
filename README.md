# Lasso Security (lasso-security)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Lasso Security is a GenAI security platform that protects every LLM and AI agent touchpoint. Its Deputy gateway inspects LLM and MCP traffic in real time, and the Classify / Threat Detection API scores prompts and completions for prompt injection, jailbreaks, PII, and harmful content, returning structured BLOCK / WARN / AUTO_MASKING findings.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- GenAI Security
- Prompt Injection
- Guardrails
- MCP

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Lasso Classify / Threat Detection API

REST API that classifies LLM prompts and completions for security violations - prompt injection, jailbreaks, harmful content, custom policies, and PII - via POST /classify, returning structured deputy findings with BLOCK / WARN / AUTO_MASKING action levels and severity. POST /classifix additionally returns PII-masked messages.

- **Human URL:** [https://www.lasso.security/platform/lasso-for-applications](https://www.lasso.security/platform/lasso-for-applications)
- **Base URL:** `https://server.lasso.security/gateway/v3`

#### Tags

- Classify
- Threat Detection
- Guardrails
- PII

#### Properties

- [Documentation](https://www.lasso.security/platform/lasso-for-applications)
- [API Reference](https://docs.litellm.ai/docs/proxy/guardrails/lasso_security)
- [OpenAPI](openapi/lasso-security-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lasso-security.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lasso-security.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lasso LLM Gateway (Deputy)

Runtime LLM firewall / gateway powered by Lasso Intent Deputies that inspects every prompt and response at the intent layer - decoding obfuscation techniques and detecting prompt injection, goal manipulation, and data leakage. Deployed in front of LLM applications via Gateway, API, or SDK and backed by the same /classify scoring engine.

- **Human URL:** [https://www.lasso.security/platform/lasso-for-applications](https://www.lasso.security/platform/lasso-for-applications)
- **Base URL:** `https://server.lasso.security/gateway/v3`

#### Tags

- Gateway
- Deputy
- LLM Firewall
- Runtime Protection

#### Properties

- [Documentation](https://www.lasso.security/platform/lasso-for-applications)
- [OpenAPI](openapi/lasso-security-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lasso-security.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lasso-security.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lasso MCP Gateway

Open-source (MIT, Python) plugin-based gateway that proxies and orchestrates Model Context Protocol (MCP) servers, intercepting requests and responses to mask secrets and PII, block prompt injection, scan server reputation, and enforce custom policies via the Lasso v3 classify API using a LASSO_API_KEY.

- **Human URL:** [https://github.com/lasso-security/mcp-gateway](https://github.com/lasso-security/mcp-gateway)
- **Base URL:** `https://server.lasso.security/gateway/v3`

#### Tags

- MCP
- Gateway
- Security Scanner
- Open Source

#### Properties

- [Documentation](https://github.com/lasso-security/mcp-gateway)
- [Documentation](https://www.lasso.security/resources/lasso-releases-first-open-source-security-gateway-for-mcp)
- [OpenAPI](openapi/lasso-security-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lasso-security.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lasso-security.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/lasso-security)
- [LinkedIn](https://www.linkedin.com/company/lasso-security)
- [Website](https://www.lasso.security/)
- [Documentation](https://www.lasso.security/platform/lasso-for-applications)
- [Plans](plans/lasso-security-plans-pricing.yml)
- [Rate Limits](rate-limits/lasso-security-rate-limits.yml)
- [Fin Ops](finops/lasso-security-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
