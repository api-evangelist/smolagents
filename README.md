# smolagents (smolagents)

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
