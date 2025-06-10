# 🚀 Local LLM API Serving with vLLM and OpenAI SDK

This repository demonstrates how to **serve a large language model (LLM)** locally using [vLLM](https://github.com/vllm-project/vllm), and **interact with it using the OpenAI SDK**. The example uses the [`google/gemma-2-2b-it`](https://huggingface.co/google/gemma-2-2b-it) model from Hugging Face.

---

## 🧠 What This Project Does

- Installs required packages: `vllm`, `huggingface_hub`, `openai`.
- Serves the `google/gemma-2-2b-it` model locally using `vllm`.
- Communicates with the local server via the OpenAI-compatible API interface.
- Generates a response to a user prompt using the locally served LLM.
