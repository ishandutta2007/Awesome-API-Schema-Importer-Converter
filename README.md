# Awesome-API-Schema-Importer-Converter

A curated collection of tools, libraries, and platforms for importing, converting, parsing, validating, and generating code from API schemas and specifications (OpenAPI, Swagger, RAML, GraphQL, Protobuf, AsyncAPI, and Postman Collections).

---

## Sector Overview & Market Dynamics

The global API management and developer tooling market is estimated at approximately **$8.0B to $10.3B** (projected to reach $22B–$37B+ by the early 2030s at a ~16–25% CAGR). The sector exhibits a **moderately fragmented** structure overall: while core infrastructure gateways and enterprise lifecycle suites are relatively concentrated among hyperscalers and legacy enterprise providers, the surrounding developer ecosystem (schema converters, mock servers, documentation platforms, and SDK generation engines) remains highly fragmented with active product-led growth and continuous startup entry.

---

## SaaS Platforms

| Product | Company Size (Valuation / Revenue) | Pricing | Free Tier Limit | Primary Capabilities & Schema Support |
| :--- | :--- | :--- | :--- | :--- |
| **[Postman](https://www.postman.com)** | **$5.6B Valuation** (~$270M–$313M ARR) | Starts at **$9/user/month** (Solo, billed annually) or $19/user/month (Team) | **Free Forever**: 1 user only, shared workspace collaboration disabled, capped at 1,000 monthly cloud requests / mock server calls / monitor runs. | API client & Spec Hub importing OpenAPI 2.0/3.0/3.1, AsyncAPI, RAML, GraphQL, WSDL, and Protocol Buffers. |
| **[Stoplight (SmartBear)](https://stoplight.io)** | **~$150M+ Parent Revenue** (Acquired by SmartBear, previously raised ~$26M) | Starts at **$44/month** (Basic plan, billed annually) | **Free Forever**: 1 user seat, 1 active design project, basic mock server, and read-only published docs. | Visual OpenAPI designer, Prism mock engine, schema validation, and spectral linting. |
| **[Speakeasy](https://www.speakeasy.com)** | **~$25.9M Funding** (Valued at ~$25M–$50M+) | Starts at **$600/month per language target** (Business plan, billed annually) | **Free Forever**: 1 language target, up to 250 operations/endpoints, manual triggers, and community support. | Automated SDK and CLI generator from OpenAPI 3.0/3.1 specs, contract validation, and AI agent toolchain generation. |
| **[Redocly](https://redocly.com)** | **~$7.8M Estimated Revenue** (Bootstrapped / Seed stage) | Starts at **$249/month** (Pro plan, billed annually) | **30-Day Free Trial**: Full Pro plan access for 30 days (up to 3 projects, unlimited seats; no permanent hosted free tier). CLI and core renderer remain free open source. | API catalog portals, OpenAPI 3.x bundler (`redocly bundle` for inlining `$ref`), linter, and markdown-integrated docs. |
| **[APIMatic](https://www.apimatic.io)** | **~$5.1M Estimated Revenue** (Bootstrapped / ~$517K Seed funding) | Starts at **$10/month** (Lite plan) or $300/month (Basic plan, billed annually) | **14-Day Free Trial**: 14 days of full feature access with no credit card required (no ongoing hosted free tier). CLI provides local validation. | Multi-format bidirectional schema transformer (OpenAPI/Swagger, RAML, API Blueprint, WSDL, Postman to OpenAPI), SDK generation. |

---

## Open-Source Converters & Generators

| Tool | Stars | Language / Tech | License | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[OpenAPITools/openapi-generator](https://github.com/OpenAPITools/openapi-generator)** | 24.4k+ | Java | Apache 2.0 | Generate client SDKs, server stubs, API documentation, and configuration from OpenAPI (v2, v3) specs across 50+ languages. |
| **[Stoplight Prism](https://github.com/stoplightio/prism)** | 4.7k+ | TypeScript / Node.js | Apache 2.0 | Turn OpenAPI v2/v3 and Postman Collections into local or hosted mock servers with dynamic response generation and schema contract validation. |
| **[Apimatic CLI](https://github.com/apimatic/apimatic-cli)** | 88+ | Node.js | Apache 2.0 | CLI for validating and transforming API definitions across 14 formats (OpenAPI 2.0/3.0, RAML, WSDL, Postman Collections, API Blueprint). |
| **[Redocly CLI](https://github.com/Redocly/redocly-cli)** | 1.1k+ | TypeScript | MIT | Swiss Army knife for OpenAPI/AsyncAPI: linting, bundling multi-file specifications, resolving external `$ref` references, and split/join workflows. |
| **[Transform.tools](https://transform.tools)** | 15.5k+ | TypeScript / React | MIT | In-browser, client-side polyglot converter supporting JSON to TypeScript, GraphQL to TypeScript/Flow, JSON Schema, and more. |
| **[speakeasy-api/openapi-generation](https://github.com/speakeasy-api/openapi-generation)** | 19+ | Go | AGPL-3.0 | Core open-source generation engine used by Speakeasy for parsing and validating OpenAPI definitions to generate production-ready code. |

---

## Categories & Workflows

1. **Schema-to-Schema Converters**: Translate between formats (e.g., RAML/WSDL/Postman Collection $\rightarrow$ OpenAPI 3.x).
2. **Schema Bundlers & Inliners**: Resolve multi-file `$ref` trees into single-file self-contained definitions (e.g., `redocly bundle`).
3. **Spec-to-Code / SDK Generators**: Parse schemas into typed client libraries, CLI tools, or server boilerplate (e.g., `openapi-generator`, `speakeasy`).
4. **Mocking & Validation Engines**: Spin up contract-adherent mock endpoints directly from API schemas (e.g., `prism`).
