# smolagents (smolagents)

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

smolagents is an open-source Python library developed by Hugging Face that enables developers to build and run powerful AI agents with minimal code — the entire agent logic fits in approximately 1,000 lines. The library provides two primary agent paradigms: **CodeAgent**, which writes actions as Python code snippets for maximum expressiveness and composability, and **ToolCallingAgent**, which uses structured JSON for reliable, validated tool interactions. smolagents is fully model-agnostic, supporting Hugging Face Inference Providers, local Transformers, Ollama, LiteLLM (100+ LLMs), Azure OpenAI, Amazon Bedrock, and MLX. Hub integration lets teams share and load agents and tools as Gradio Spaces, and multi-agent orchestration enables hierarchical systems where manager agents coordinate specialized sub-agents.

APIs.json: [https://raw.githubusercontent.com/api-evangelist/smolagents/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/smolagents/refs/heads/main/apis.yml)

Naftiko: [https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=smolagents-api-evangelist&utm_content=repo](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=smolagents-api-evangelist&utm_content=repo)

## Tags

- AI Agents
- Multi-Agent
- Python
- Code Generation
- LLM
- Hugging Face
- Open Source
- Machine Learning

## APIs

| Name | Description | Human URL |
|------|-------------|-----------|
| smolagents Python Library | CodeAgent and ToolCallingAgent classes for building AI agents that write Python code or structured JSON to call tools, with Hub integration and multi-agent orchestration. | [https://huggingface.co/docs/smolagents/en/index](https://huggingface.co/docs/smolagents/en/index) |

## Plans, Rate Limits, and FinOps

| Resource | URL |
|----------|-----|
| Plans & Pricing | [plans/smolagents-plans-pricing.yml](plans/smolagents-plans-pricing.yml) |
| Rate Limits | [rate-limits/smolagents-rate-limits.yml](rate-limits/smolagents-rate-limits.yml) |
| FinOps | [finops/smolagents-finops.yml](finops/smolagents-finops.yml) |

**Key pricing facts:**
- smolagents library is free (Apache 2.0)
- Free Hugging Face account: $0.10/month inference credits
- PRO ($9/month): $2.00/month inference credits, higher rate limits
- Team ($20/user/month): $2.00/seat inference credits, SSO, Audit Logs
- Enterprise ($50/user/month): highest limits, SCIM, dedicated support
- Pay-as-you-go inference: provider cost passed through at no markup

**Key rate limits (per 5-minute fixed window):**

| Plan | Hub API | Resolvers | Pages |
|------|---------|-----------|-------|
| Anonymous | 500 | 3,000 | 100 |
| Free | 1,000 | 5,000 | 200 |
| PRO | 2,500 | 12,000 | 400 |
| Team | 3,000 | 20,000 | 400 |
| Enterprise | 6,000 | 50,000 | 600 |
| Enterprise Plus | 10,000 | 100,000 | 1,000 |

HTTP 429 is returned when rate limits are exceeded. The `huggingface_hub` library (v1.2.0+) auto-retries on 429 by parsing the `RateLimit` header.

## Timestamps

- **Created:** 2026-06-12
- **Modified:** 2026-06-12

## Common Properties

| Type | URL |
|------|-----|
| Website | [https://huggingface.co/smolagents](https://huggingface.co/smolagents) |
| Documentation | [https://huggingface.co/docs/smolagents/en/index](https://huggingface.co/docs/smolagents/en/index) |
| GitHub Organization | [https://github.com/huggingface](https://github.com/huggingface) |
| GitHub Repository | [https://github.com/huggingface/smolagents](https://github.com/huggingface/smolagents) |
| Blog | [https://huggingface.co/blog/smolagents](https://huggingface.co/blog/smolagents) |
| Changelog | [https://github.com/huggingface/smolagents/releases](https://github.com/huggingface/smolagents/releases) |
| PyPI | [https://pypi.org/project/smolagents/](https://pypi.org/project/smolagents/) |
| Pricing | [https://huggingface.co/pricing](https://huggingface.co/pricing) |
| Status Page | [https://status.huggingface.co](https://status.huggingface.co) |
| X (Twitter) | [https://x.com/huggingface](https://x.com/huggingface) |
| LinkedIn | [https://www.linkedin.com/company/huggingface](https://www.linkedin.com/company/huggingface) |

## Maintainers

| Name | Email |
|------|-------|
| Kin Lane | kin@apievangelist.com |
