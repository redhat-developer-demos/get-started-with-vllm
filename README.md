# Get Started with vLLM

Hands-on notebooks for compressing, serving, and benchmarking LLMs with [vLLM](https://docs.vllm.ai/) — built for the [Red Hat OpenShift AI Developer Sandbox](https://developers.redhat.com/developer-sandbox).

## Notebooks

| # | Folder | Notebook | What you'll do |
|---|--------|----------|----------------|
| 1 | `llm-compression/` | **Optimizing a Model with LLM Compressor** | Apply GPTQ W4A16 quantization to Qwen3-0.6B and compare it against the original |
| 2 | `vllm-inference/` | **Serving LLMs Efficiently with vLLM** | Query a vLLM server with the OpenAI-compatible API, explore logprobs, continuous batching, KV cache metrics, and prefix caching |
| 3 | `benchmarks-evals/` | **Measuring What Matters: Benchmarking and Evaluation** | Run GuideLLM serving benchmarks and lm_eval quality checks, then decide if a quantization tradeoff is worth deploying |

The recommended flow is **1 → 2 → 3**, but each notebook is self-contained — pick whichever topic interests you.

> **Note:** Pre-quantized models are already included in `llm-compression/` so you can skip straight to inference or benchmarking if you prefer.

## Prerequisites

- A free [Developer Sandbox](https://developers.redhat.com/developer-sandbox) account
- An **OpenShift API token** (used as your LLM API key) — follow the [sandbox LLM guide](https://developers.redhat.com/learning/learn:ai:get-started-consuming-gpu-hosted-large-language-models-developer-sandbox/resource/resources:interact-gpu-hosted-models-using-jupyter-notebook-and-langchain) to retrieve it

## Getting started

1. Open **OpenShift AI** from the Developer Sandbox and create a workbench using the **Jupyter Minimal — CPU — Python 3.12** image.
2. Clone this repo inside the workbench:
   ```bash
   git clone https://github.com/<org>/get-started-with-vllm.git
   ```
3. Open the notebook you want, install its dependencies (`pip install -r requirements.txt` in the matching folder), and run the cells.

## License

[Apache 2.0](LICENSE)
