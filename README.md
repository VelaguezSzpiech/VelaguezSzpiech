# Hey, I'm Velaguez 👋

**AI Systems Engineer · Process Optimization & Automation · Local Inference Builder**

I build high-efficiency AI systems, custom automation pipelines, and bare-metal tooling. I started out in full-stack development, got hooked on squeezing every last drop of performance out of hardware I already own, and now spend most of my time at the intersection of **local AI infrastructure**, **agentic workflows**, and **process optimization**.

---

## 🎯 What I Focus On

- **AI Integration & Automation** — Designing end-to-end workflows and agentic pipelines that remove manual bottlenecks and turn repetitive processes into fast, reliable systems.
- **Bare-Metal Inference & Performance** — Writing low-level GPU kernels, optimizing memory bandwidth, and pushing local hardware way past stock baselines.
- **Open-Source & Local-First Tooling** — Contributing to and building transparent, self-hosted tools so developers can own their stack and their weights.
- **Process Optimization** — Auditing systems from top to bottom—whether it's an inference hot path or an operational workflow—to cut latency, waste, and overhead.

---

## 🚀 Featured Project: [VegaJet](https://github.com/VelaguezSzpiech/vegajet)

A bare-metal Linux `/dev/kfd` LLM inference engine built from scratch for AMD Instinct MI50 (`gfx906`) accelerators—zero ROCm runtime dependency.

- **Bare-Metal Architecture:** Direct `/dev/kfd` AQL queues, custom persistent `gfx906` kernels with 0 B register spills, and Push-Only Dual-BAR PCIe P2P AllReduce.
- **Universal Load-Time Repacker:** Translates GGUF weights on load into native `gfx906` layouts (`v_dot4_i32_i8` / `v_dot8_i32_i4`) to maximize HBM2 saturation.
- **Real-World Speed:** Running a 122B MoE (`Ornith-122B`) across 2× 32 GB MI50s at **~165 tok/s raw decode**, **311–357 tok/s** with lossless Hybrid speculative decoding on code, and **1,345+ tok/s prefill**.
- **Drop-In Serving:** Native OpenAI- and Anthropic-compatible (`/v1/chat/completions` & `/v1/messages`) streaming server so existing clients and harnesses plug right in.

---

## 🛠️ Building in the Background

- **Hermes & OMP Harnesses** — Developing custom orchestration and execution harnesses to wire local and frontier models into automated engineering and workflow pipelines.
- **Multi-GPU Scaling & Universal Model Support** — Expanding VegaJet for 3×+ MI50 setups, broader GGUF architecture coverage, and zero-config hardware auto-tuning.

---

## 🧰 Tech Stack

- **Systems & Inference:** `C++` · `HIP / gfx906` · `Linux /dev/kfd` · `GGUF` · `Speculative Decoding`
- **AI & Automation:** `Local LLMs` · `AI Integration` · `Agentic Harnesses (Hermes / OMP)` · `Workflow & Process Optimization`
- **Full-Stack & Scripting:** `Python` · `Node.js` · `TypeScript` · `React` · `Vite`
