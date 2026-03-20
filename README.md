<p align="center">
  <img src="banner.png" alt="Free Inference Banner" width="100%">
</p>

<h1 align="center">Free Inference</h1>

<p align="center">
  A comprehensive guide to free AI/LLM inference APIs — no credit card required, no expiry.
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License: MIT"></a>
  <img src="https://img.shields.io/badge/last%20updated-March%202026-brightgreen" alt="Last Updated">
  <img src="https://img.shields.io/badge/free%20models-81%2B-orange" alt="Free Models">
  <img src="https://img.shields.io/badge/providers-20%2B-purple" alt="Providers">
</p>

<p align="center">
  Sources: <a href="https://models.dev">models.dev</a> · <a href="https://github.com/BerriAI/litellm/blob/main/model_prices_and_context_window.json">LiteLLM Pricing JSON</a> · Community Research
</p>

---

## Table of Contents

- [Tier 1: Truly Free (No Credit Card)](#tier-1-truly-free-no-credit-card-no-expiry)
- [Tier 2: Free Credits / Trial](#tier-2-free-credits--trial-may-require-card)
- [Tier 3: Self-Hosted](#tier-3-self-hosted-always-free-you-provide-compute)
- [Tier 4: Chat-Only (No API)](#tier-4-chat-only-no-api)
- [Quick Comparison by Use Case](#quick-comparison-best-free-options-by-use-case)
- [OpenAI-Compatible Endpoints](#openai-compatible-endpoints)
- [LiteLLM Verified Free Models](#litellm-verified-free-models-0-input--0-output)
- [LiteLLM Integration](#litellm-integration)
- [Contributing](#contributing)

---

## Tier 1: Truly Free (No Credit Card, No Expiry)

### Google AI Studio

| Model | RPM | Daily Cap | Context | Features |
|-------|-----|-----------|---------|----------|
| Gemini 2.5 Pro | 5 | 100 req | 1M | Vision, function calling |
| Gemini 2.5 Flash | 15 | 500 req | 1M | Vision, function calling |
| Gemini 2.5 Flash-Lite | 15 | 1,000 req | 1M | Vision |
| Gemini 2.0 Flash | 15 | 1,500 req | 1M | Vision, function calling |
| Gemma 3 27B | 15 | — | 128K | Vision, function calling |

- **Sign-up:** [ai.google.dev](https://ai.google.dev) (Google account)
- **OpenAI-compatible:** Yes
- **Multimodal:** Yes (text, image, video, audio)

### Groq

| Model | RPM | Daily Cap | Speed |
|-------|-----|-----------|-------|
| Llama 3.3 70B | 30 | 1,000 req | ~500 tok/s |
| Llama 4 Scout | 30 | 1,000 req | ~500 tok/s |
| Qwen3 32B | 30 | 14,400 req | ~750 tok/s |
| Kimi K2 | 30 | 1,000 req | ~500 tok/s |
| Gemma 2 9B | 30 | 14,400 req | ~750 tok/s |

- **Sign-up:** [console.groq.com](https://console.groq.com)
- **OpenAI-compatible:** Yes
- **Highlight:** Fastest inference speeds in the industry (custom LPU hardware)

### OpenRouter

| Model | Context | Max Output |
|-------|---------|------------|
| GPT-OSS 120B | 131K | 131K |
| Qwen3 Coder 480B (MoE) | 262K | 262K |
| NVIDIA Nemotron 3 Super 120B | 262K | 262K |
| Llama 3.3 70B | 65K | — |
| Hermes 3 Llama 3.1 405B | 131K | — |
| DeepSeek R1/V3 | 128K | — |
| Llama 4 Maverick/Scout | 128K+ | — |
| MiniMax M2.5 | 196K | 196K |
| Step 3.5 Flash | 256K | 256K |
| Mistral Small 3.1 24B | 128K | — |
| Gemma 3 (27B/12B/4B) | 32-131K | 8K |
| 15+ more models | — | — |

- **Sign-up:** [openrouter.ai](https://openrouter.ai)
- **Rate limits:** ~20 RPM, 50 req/day (free), 1,000 req/day (with $10+ balance)
- **Usage:** Append `:free` to model IDs (e.g., `meta-llama/llama-3.3-70b-instruct:free`)
- **Highlight:** Single API key, 27+ free models from multiple providers

### Cerebras

| Model | RPM | Daily Cap |
|-------|-----|-----------|
| Llama 3.3 70B | 30 | 1M tok/day |
| Qwen3 32B | 30 | 1M tok/day |
| Qwen3 235B | 30 | 1M tok/day |
| GPT-OSS 120B | 30 | 1M tok/day |

- **Sign-up:** [cloud.cerebras.ai](https://cloud.cerebras.ai)
- **OpenAI-compatible:** Yes
- **Highlight:** Wafer-scale engine, extremely fast inference

### Mistral AI

| Model | RPM | Monthly Cap |
|-------|-----|-------------|
| Mistral Large | 2 | 1B tokens |
| Mistral Small | 2 | 1B tokens |
| Codestral | 2 | 1B tokens |
| Pixtral 12B | 2 | 1B tokens |

- **Sign-up:** [console.mistral.ai](https://console.mistral.ai)
- **Highlight:** Codestral is specifically free for code generation tasks

### Cloudflare Workers AI

| Model | Daily Cap |
|-------|-----------|
| Llama 3.2 | 10K neurons |
| Mistral 7B | 10K neurons |
| FLUX.2 (image gen) | 10K neurons |
| Whisper (speech-to-text) | 10K neurons |

- **Sign-up:** [dash.cloudflare.com](https://dash.cloudflare.com)
- **Highlight:** Edge deployment with global low-latency

### GitHub Models

| Model | RPM | Daily Cap | Token Limits |
|-------|-----|-----------|--------------|
| GPT-4o | 10 | 50 req | 8K in / 4K out |
| GPT-4.1 | 10 | 50 req | 8K in / 4K out |
| o3 | 10 | 50 req | 8K in / 4K out |
| Grok-3 | 10 | 50 req | 8K in / 4K out |
| DeepSeek-R1 | 10 | 50 req | 8K in / 4K out |

- **Sign-up:** [github.com/marketplace/models](https://github.com/marketplace/models) (GitHub account)
- **Highlight:** Playground UI included, access to proprietary models for free

### Cohere

| Model | Monthly Cap | RPM |
|-------|-------------|-----|
| Command R+ | 1,000 req | 20 |
| Embed 4 | 1,000 req | 20 |
| Rerank 3.5 | 1,000 req | 20 |

- **Sign-up:** [dashboard.cohere.com](https://dashboard.cohere.com)
- **Highlight:** Full RAG pipeline (generation + embedding + reranking)

### HuggingFace Inference API

- **Models:** 300+ community-hosted models (up to ~10B params on free tier)
- **Limits:** Variable, cold-start delays possible (30+ sec)
- **Sign-up:** [huggingface.co](https://huggingface.co)
- **Highlight:** Long-tail/specialized model access

### NVIDIA NIM

94 free endpoint models across NVIDIA and third-party providers. Key chat/completion models:

**NVIDIA Models**

| Model | Type | Details |
|-------|------|---------|
| Nemotron 3 Super 120B (A12B) | Chat | 1M context, downloadable |
| Nemotron 3 Nano 30B (A3B) | Chat | 1M context, downloadable |
| Llama 3.3 Nemotron Super 49B v1.5 | Chat | Free endpoint |
| Llama 3.1 Nemotron Nano 4B v1.1 | Chat | Free endpoint |
| Nemotron Mini 4B Instruct | Chat | Free endpoint |
| Nemotron Nano 12B v2 VL | Multimodal | Vision + chat |
| Mistral Nemo Minitron 8B | Language | Free endpoint |

**DeepSeek Models**

| Model | Details |
|-------|---------|
| DeepSeek V3.2 (685B) | Sparse attention, long context, agentic tools |
| DeepSeek V3.1 Terminus | 128K context, think/non-think modes, function calling |
| DeepSeek V3.1 | 128K context, fast reasoning, tool use |
| DeepSeek R1 Distill (Qwen 32B/14B/7B, Llama 8B) | Downloadable |

**Qwen Models**

| Model | Details |
|-------|---------|
| Qwen 3.5 122B (A10B MoE) | Coding, reasoning, multimodal, agent-ready |
| Qwen3 Coder 480B (A35B) | 256K context, agentic coding |
| QwQ 32B | Reasoning model |
| Qwen 2.5 Coder 7B Instruct | 32K context |
| Qwen 2 7B Instruct | Free endpoint |

**Meta Llama Models**

| Model | Details |
|-------|---------|
| Llama 4 Maverick 17B (128E MoE) | Multimodal, multilingual |
| Llama 4 Scout 17B (16E MoE) | Multimodal, multilingual |
| Llama Guard 4 12B | Safety classification |

**Mistral AI Models**

| Model | Details |
|-------|---------|
| Mistral Large 3 675B (MoE VLM) | Chat, agentic, multimodal |
| Devstral 2 123B | 256K context, code + deep reasoning |
| Magistral Small | Reasoning, edge deployment |
| Mistral Nemotron | Agentic workflows, function calling |
| Mistral Small 3.1 24B | Multilingual, image understanding |
| Mistral Medium 3 | Enterprise, software dev |
| Mamba Codestral 7B | Code generation |
| Mixtral 8x22B Instruct | MoE, general purpose |

**Google Models**

| Model | Details |
|-------|---------|
| Gemma 3N E4B/E2B | Edge computing, multimodal (text/audio/image) |
| Gemma 3 27B IT | Multimodal reasoning from images |
| Gemma 2 27B/2B IT | Text generation, code |
| PaliGemma | Vision-language model |
| ShieldGemma 9B | Safety guardrail |
| Gemma 7B | Text generation |

- **Sign-up:** [build.nvidia.com](https://build.nvidia.com) (1,000 free credits, up to 5,000)
- **Rate limits:** ~40 RPM
- **Highlight:** 94 free endpoints + self-hosted Docker containers via NIM microservices

---

## Tier 2: Free Credits / Trial (May Require Card)

| Provider | Models | Free Credits | Card Required | Validity |
|----------|--------|-------------|---------------|----------|
| **xAI** | Grok 4, Grok 4.1 Fast (2M ctx) | $25 | No (initially) | — |
| **DeepSeek** | V3, R1 | 5M tokens | No | 30 days |
| **SambaNova** | Llama 3.3 70B, 3.1 405B, Qwen 2.5 72B | $5 + free tier after | No | 30 days (credits) |
| **Together AI** | Llama 4 Scout, DeepSeek R1 | $5 min purchase | Yes | — |
| **Fireworks AI** | Llama 3.1 405B, DeepSeek R1, 100+ models | $1 | No | — |
| **AI21 Labs** | Jamba Large, Jamba Mini | $10 | No | 3 months |
| **Anthropic** | Claude Sonnet, Claude Opus | $5 | No | One-time |
| **OpenAI** | GPT-4o, GPT-4.1 | $5 | No | — |

---

## Tier 3: Self-Hosted (Always Free, You Provide Compute)

### Ollama

Run models locally with zero API costs.

| Model | RAM Required |
|-------|-------------|
| DeepSeek V3.1 671B | 384GB+ |
| Qwen3 Coder 480B | 256GB+ |
| GPT-OSS 120B | 80GB+ |
| Llama 3.3 70B | 48GB |
| Qwen 2.5 72B | 48GB |
| Mistral Small 3.1 | 16GB |
| Phi-4 | 12GB |
| Gemma 2 9B | 8GB |

- **Install:** [ollama.com](https://ollama.com)

### Lemonade (Edge / On-Device)

GGUF-quantized models for edge inference: Gemma 3 4B, Qwen3 4B, Qwen3 Coder 30B (MoE), GPT-OSS 20B.

---

## Tier 4: Chat-Only (No API)

| Service | Model | Limits |
|---------|-------|--------|
| ChatGPT Free | GPT-5.2 | Daily message cap, ad-supported |
| Claude Free | Claude Sonnet | Daily message cap |
| Gemini Free | Gemini 3 Pro | Google Workspace integration |
| Microsoft Copilot | GPT-5.2 | Free DALL-E image gen |
| Perplexity Free | Search-augmented | Limited daily queries |

---

## Quick Comparison: Best Free Options by Use Case

| Use Case | Best Provider | Why |
|----------|--------------|-----|
| **Largest context window** | Google AI Studio (1M), xAI Grok (2M) | Unmatched context for long documents |
| **Fastest inference** | Groq, Cerebras | Custom silicon, 500+ tok/s |
| **Most model variety** | OpenRouter (27+ free models) | One API key, many providers |
| **Code generation** | Mistral Codestral, Qwen3 Coder (OpenRouter) | Purpose-built for code |
| **RAG pipelines** | Cohere (gen + embed + rerank) | Full pipeline in one provider |
| **Highest daily volume** | Cloudflare Workers AI (10K/day) | Best for high-throughput prototyping |
| **Proprietary models for free** | GitHub Models (GPT-4.1, o3, Grok-3) | Access to closed-source models |
| **Privacy / offline** | Ollama (self-hosted) | Data never leaves your machine |
| **Production-grade free** | Google AI Studio | Most generous limits + best models |

---

## OpenAI-Compatible Endpoints

Most providers support the OpenAI SDK format, making it easy to swap providers:

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://PROVIDER_BASE_URL",
    api_key="YOUR_FREE_API_KEY",
)

response = client.chat.completions.create(
    model="MODEL_NAME",
    messages=[{"role": "user", "content": "Hello!"}],
)
```

| Provider | Base URL |
|----------|----------|
| Google AI Studio | `https://generativelanguage.googleapis.com/v1beta/openai/` |
| Groq | `https://api.groq.com/openai/v1` |
| OpenRouter | `https://openrouter.ai/api/v1` |
| Cerebras | `https://api.cerebras.ai/v1` |
| Mistral | `https://api.mistral.ai/v1` |
| Together AI | `https://api.together.xyz/v1` |
| Fireworks AI | `https://api.fireworks.ai/inference/v1` |
| NVIDIA NIM | `https://integrate.api.nvidia.com/v1` |

---

## LiteLLM Verified Free Models ($0 Input / $0 Output)

> Data from [`model_prices_and_context_window.json`](https://github.com/BerriAI/litellm/blob/main/model_prices_and_context_window.json) — 81 free chat/completion models across 16 providers.

### Cloud API Providers

| Provider | Model (LiteLLM ID) | Context | Max Output | Vision | Function Calling |
|----------|---------------------|---------|------------|--------|-----------------|
| **Gemini** | `gemini/gemini-exp-1206` | 2M | 8K | Yes | Yes |
| | `gemini/gemini-exp-1114` | 1M | 8K | Yes | Yes |
| | `gemini/gemma-3-27b-it` | 131K | 8K | Yes | Yes |
| | `gemini/learnlm-1.5-pro-experimental` | 32K | 8K | Yes | Yes |
| **Codestral** | `codestral/codestral-2405` | 32K | 8K | — | — |
| | `codestral/codestral-latest` | 32K | 8K | — | — |
| **OpenRouter** | `openrouter/openrouter/auto` | 2M | — | Yes | Yes |
| | `openrouter/openrouter/free` | 200K | — | Yes | Yes |
| | `openrouter/openrouter/bodybuilder` | 128K | — | — | — |
| **Together AI** | `together_ai/meta-llama/Llama-3.3-70B-Instruct-Turbo-Free` | — | — | — | Yes |
| **Vertex AI** | `vertex_ai/meta/llama3-405b-instruct-maas` | 32K | 32K | — | — |
| | `vertex_ai/meta/llama-3.2-90b-vision-instruct-maas` | 128K | 2K | Yes | — |
| | `vertex_ai/meta/llama-3.1-70b-instruct-maas` | 128K | 2K | Yes | — |
| | `vertex_ai/meta/llama-3.1-8b-instruct-maas` | 128K | 2K | Yes | — |
| | `vertex_ai/meta/llama3-70b-instruct-maas` | 32K | 32K | — | — |
| | `vertex_ai/meta/llama3-8b-instruct-maas` | 32K | 32K | — | — |
| **Volcengine** | `deepseek-v3-2-251201` | 98K | 32K | — | Yes |
| | `glm-4-7-251222` | 204K | 131K | — | Yes |
| | `kimi-k2-thinking-251104` | 229K | 32K | — | Yes |
| **GigaChat** | `gigachat/GigaChat-2-Max` | 128K | 8K | Yes | Yes |
| | `gigachat/GigaChat-2-Pro` | 128K | 8K | Yes | Yes |
| | `gigachat/GigaChat-2-Lite` | 128K | 8K | — | Yes |
| **PublicAI** | `publicai/allenai/Olmo-3-32B-Think` | 32K | 4K | — | Yes |
| | `publicai/aisingapore/Qwen-SEA-LION-v4-32B-IT` | 32K | 4K | — | Yes |
| | `publicai/allenai/Olmo-3-7B-Think` | 32K | 4K | — | Yes |
| | `publicai/allenai/Olmo-3-7B-Instruct` | 32K | 4K | — | Yes |
| | `publicai/BSC-LT/ALIA-40b-instruct_Q8_0` | 8K | 4K | — | Yes |
| | `publicai/swiss-ai/apertus-70b-instruct` | 8K | 4K | — | — |
| | + 3 more models | | | | |
| **ZAI** | `zai/glm-4.5-flash` | 128K | 32K | — | Yes |
| **Sarvam** | `sarvam/sarvam-m` | 8K | 32K | — | — |

### Self-Hosted / Edge (Always $0)

| Provider | Model (LiteLLM ID) | Context | Max Output |
|----------|---------------------|---------|------------|
| **Ollama** | `ollama/deepseek-v3.1:671b-cloud` | 163K | 163K |
| | `ollama/qwen3-coder:480b-cloud` | 262K | 262K |
| | `ollama/gpt-oss:120b-cloud` | 131K | 131K |
| | `ollama/mixtral-8x22B-Instruct-v0.1` | 65K | 65K |
| | `ollama/mistral-large-instruct-2407` | 65K | 8K |
| | `ollama/llama3.1` | 8K | 8K |
| | + 23 more models | | |
| **Lemonade** | `lemonade/Qwen3-Coder-30B-A3B-Instruct-GGUF` | 262K | 32K |
| | `lemonade/gpt-oss-120b-mxfp-GGUF` | 131K | 32K |
| | `lemonade/Qwen3-4B-Instruct-2507-GGUF` | 262K | 32K |
| | `lemonade/gpt-oss-20b-mxfp4-GGUF` | 131K | 32K |
| | `lemonade/Gemma-3-4b-it-GGUF` | 128K | 8K |

---

## LiteLLM Integration

Use [LiteLLM](https://github.com/BerriAI/litellm) as a unified proxy to route across all these providers with a single interface:

```python
import litellm

# Google Gemini (free)
response = litellm.completion(model="gemini/gemini-exp-1206", messages=[...])

# OpenRouter free router
response = litellm.completion(model="openrouter/openrouter/free", messages=[...])

# Volcengine DeepSeek V3 (free)
response = litellm.completion(model="deepseek-v3-2-251201", messages=[...])

# Together AI Llama (free)
response = litellm.completion(model="together_ai/meta-llama/Llama-3.3-70B-Instruct-Turbo-Free", messages=[...])

# Vertex AI Llama 405B (free MaaS preview)
response = litellm.completion(model="vertex_ai/meta/llama3-405b-instruct-maas", messages=[...])

# Codestral (free for code)
response = litellm.completion(model="codestral/codestral-latest", messages=[...])
```

---

## Contributing

Found a new free provider or spotted outdated info? Open an issue or PR.

## License

MIT
