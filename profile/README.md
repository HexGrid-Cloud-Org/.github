
# HexGrid — Private AI Cloud

Dedicated GPUs by the hour and private LLM endpoints. Your models, your
hardware, your data. Nothing shared, nothing logged.

[Rent a GPU](https://hexgrid.cloud/dashboard/deployments/deploy-pod) ·
[Deploy an LLM](https://hexgrid.cloud/dashboard/deployments/deploy-llm) ·
[Docs](https://docs.hexgrid.cloud) ·
[Pricing](https://hexgrid.cloud/pricing)

---

## Rent a GPU

Dedicated hardware by the hour, SSH access, full root. Bring any container,
notebook, or CUDA stack.

| GPU | VRAM | From |
|---|---|---|
| H100 SXM | 80 GB | $2.49/hr |
| A100 | 80 GB | $1.29/hr |
| L40S | 48 GB | $0.90/hr |

B200 and H200 class also available. See [full GPU pricing](https://hexgrid.cloud/pricing).

## Deploy a private LLM

Pick a model, pick a GPU, get a private HTTPS endpoint. We handle driver,
CUDA, and inference-engine alignment so your runtime starts correctly the
first time.

| Model | Provider | Good for |
|---|---|---|
| Llama 3.3 70B | Meta | Complex reasoning, RAG, enterprise chat |
| Gemma 4 31B | Google | General assistant workloads |
| Nemotron-3 Nano | NVIDIA | Fast, low-cost reasoning and code |
| Devstral Small 24B | Mistral | Coding agents |

[Browse all models](https://hexgrid.cloud/models)

### OpenAI-compatible from day one

Change `base_url` and your key. Nothing else.

```bash
curl https://api.hexgrid.cloud/v1/chat/completions \
  -H "Authorization: Bearer $HEXGRID_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "llama-3.3-70b-instruct",
    "messages": [{"role": "user", "content": "Explain private GPU inference."}]
  }'
```

## Private ComfyUI

Pre-provisioned MiniMax H3, Wan 2.2, and LTX Video on a box only you can
reach. Weights, custom nodes, and persistent output folders ready at launch.

## What's here

- **[open-llm-benchmarks](https://github.com/hexgrid-cloud/open-llm-benchmarks)**
  — TTFT, TPOT, throughput, latency, and cost-per-token for open models
  across dedicated GPUs. Reproducible, open methodology.

## Infrastructure

Partner datacenters are SOC 2 Type II, ISO 27001, and GDPR compliant.
Regions in US, EU, and APAC. 200+ GPUs across providers.

---

[hexgrid.cloud](https://hexgrid.cloud) ·
[Docs](https://docs.hexgrid.cloud) ·
[Blog](https://blog.hexgrid.cloud) ·
[Status](https://hexgrid.cloud/status-page) ·
[@hexgrid_cloud](https://x.com/hexgrid_cloud) ·
[HuggingFace](https://huggingface.co/hexgrid-cloud) ·
contact@hexgrid.cloud
