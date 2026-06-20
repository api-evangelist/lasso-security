# Lasso Security (lasso-security)

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
