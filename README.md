# Morph (morph-labs)

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
