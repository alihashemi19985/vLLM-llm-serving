# 🚀 Local LLM API Serving with vLLM and OpenAI SDK

This repository demonstrates how to **serve a large language model (LLM)** locally using [vLLM](https://github.com/vllm-project/vllm), and **interact with it using the OpenAI SDK**. The example uses the [`google/gemma-2-2b-it`](https://huggingface.co/google/gemma-2-2b-it) model from Hugging Face.

---

## 🧠 What This Project Does

- Installs required packages: `vllm`, `huggingface_hub`, `openai`.
- Serves the `google/gemma-2-2b-it` model locally using `vllm`.
- Communicates with the local server via the OpenAI-compatible API interface.
- Generates a response to a user prompt using the locally served LLM.


## 🧩 What is vLLM and Why Use It?
vLLM is a high-performance and easy-to-use inference engine for large language models (LLMs). It is designed to serve LLMs with high throughput and low latency — ideal for both research and production environments.

✅ Key Benefits of Using vLLM for LLM Serving:
PagedAttention Technology: vLLM introduces PagedAttention, an efficient attention algorithm that enables serving multiple concurrent requests without re-computing key-value caches. This improves memory usage and speed significantly.

OpenAI-Compatible API: You can serve your own model and access it via the OpenAI API interface, allowing easy integration with existing tools like the openai Python package.

Multi-Model and Streaming Support: vLLM supports multi-model deployment, token streaming, and advanced sampling options out of the box.

GPU Optimization: It uses GPU resources efficiently to support large models with minimal hardware requirements (compared to traditional inference setups).

Production Ready: Supports deployment at scale with features like token-based authentication, rate limiting, and distributed serving.

📌 Why It Matters in This Project:
In this project, vllm is used to:

Load and serve the google/gemma-2-2b-it model locally.

Provide a local OpenAI-compatible REST API endpoint (http://localhost:8000).

Allow interaction via the OpenAI SDK without requiring internet-based model APIs (e.g., OpenAI or Hugging Face APIs).

Enable fast and efficient inference, suitable for projects where cost, speed, and data privacy are important.
