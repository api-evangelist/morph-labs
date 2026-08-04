# Morph (morph-labs)

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

Morph builds fast models that improve AI coding agents. Its OpenAI-compatible API serves the Apply (Fast Apply) model that deterministically merges LLM-generated code edits into source files at 10,500+ tokens/second, plus code embeddings and reranking. Morph Cloud adds Infinibranch microVM sandboxes that snapshot, branch, and restore entire VM states in under 250ms for agent workloads.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/apis.yml)

## Tags

- AI
- Code Editing
- Fast Apply
- Embeddings
- Sandboxes

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Morph Apply API

OpenAI-compatible chat-completions endpoint that merges an LLM's update snippet into the original source with structure awareness, using the morph-v3-fast, morph-v3-large, and auto models. Requests carry XML-tagged instruction, code, and update content; the response is the fully merged file ready to write to disk.

- **Human URL:** [https://docs.morphllm.com/api-reference/endpoint/apply](https://docs.morphllm.com/api-reference/endpoint/apply)
- **Base URL:** `https://api.morphllm.com/v1`

#### Tags

- Apply
- Fast Apply
- Code Editing

#### Properties

- [Documentation](https://docs.morphllm.com/quickstart)
- [API Reference](https://docs.morphllm.com/api-reference/endpoint/apply)
- [OpenAPI](openapi/morph-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/morph-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/morph-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Morph Embeddings API

OpenAI-compatible embeddings endpoint producing vectors tuned for code and retrieval, using the morph-embedding-v4 model with float or base64 encoding.

- **Human URL:** [https://docs.morphllm.com/api-reference/endpoint/embedding](https://docs.morphllm.com/api-reference/endpoint/embedding)
- **Base URL:** `https://api.morphllm.com/v1`

#### Tags

- Embeddings
- Vectors
- Code

#### Properties

- [Documentation](https://docs.morphllm.com/api-reference/endpoint/embedding)
- [API Reference](https://docs.morphllm.com/api-reference/endpoint/embedding)
- [OpenAPI](openapi/morph-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/morph-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/morph-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Morph Rerank API

Cohere-client-compatible reranking endpoint that scores documents (or embedding IDs) against a query for code-aware retrieval, using the morph-rerank-v3 model with optional top_n truncation.

- **Human URL:** [https://docs.morphllm.com/models/rerank](https://docs.morphllm.com/models/rerank)
- **Base URL:** `https://api.morphllm.com/v1`

#### Tags

- Rerank
- Search
- Retrieval

#### Properties

- [Documentation](https://docs.morphllm.com/models/rerank)
- [OpenAPI](openapi/morph-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/morph-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/morph-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Morph Cloud Sandboxes API

Infinibranch microVM (Firecracker) sandbox infrastructure for agents - a user-scoped API for managing instances and snapshots with sub-250ms branch, snapshot, and restore, command exec (including SSE), and HTTP service exposure. Available via the morphcloud Python and TypeScript SDKs and CLI.

- **Human URL:** [https://cloud.morph.so/docs/developers](https://cloud.morph.so/docs/developers)
- **Base URL:** `https://cloud.morph.so/api`

#### Tags

- Sandboxes
- microVM
- Infinibranch

#### Properties

- [Documentation](https://cloud.morph.so/docs/developers)
- [API Reference](https://cloud.morph.so/docs/api-reference)

## Common Properties

- [GitHub Organization](https://github.com/morphllm)
- [GitHub Organization](https://github.com/morph-labs)
- [LinkedIn](https://www.linkedin.com/company/morph-labs)
- [Website](https://morphllm.com/)
- [Documentation](https://docs.morphllm.com)
- [Plans](plans/morph-labs-plans-pricing.yml)
- [Rate Limits](rate-limits/morph-labs-rate-limits.yml)
- [Fin Ops](finops/morph-labs-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
