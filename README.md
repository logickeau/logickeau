<h1 align="center">Jean "Nick" Pijeau</h1>
<p align="center">
  <strong>AI Security &amp; Integrity Engineer</strong><br>
  I build <strong>Vitnify</strong>, a deterministic LLM engine (bit-identical across CPUs and GPUs)
  and tamper-evident, offline-verifiable execution receipts for AI agents.
</p>

<p align="center">
  <a target="_blank" href="https://vitnify.com">vitnify.com</a> ·
  <a target="_blank" href="https://www.linkedin.com/in/jean-n-pijeau">LinkedIn</a> ·
  Orlando, FL
</p>

---

### 🔭 What I'm building

**[Vitnify](https://vitnify.com)** is my answer to the question I spent 15 years asking as a threat hunter: *what actually happened?* It lets you re-run an AI agent's model and get bit-identical output, then check a signed record of the whole run offline. Built end to end:

- 🧠 **[vitni-tensor](https://github.com/vitnify/vitni-tensor):** a deterministic, `no_std` Rust inference engine with **bit-identical** LLM output across CPU vendors, instruction sets, and GPUs. Verified byte-for-byte on Apple, AWS Graviton, Intel, AMD, Metal, and CUDA (pinned-order reductions + exact-integer k-quant kernels).
- 📜 **[vitnify](https://github.com/vitnify/vitnify)** + **[vitnify-receipt-spec](https://github.com/vitnify/vitnify-receipt-spec)**: an open protocol and SDK for **tamper-evident, offline-verifiable** agent execution receipts (BLAKE3 Merkle + ed25519), with LangGraph and MCP drop-ins. `pip install vitnify`.
- ✅ **[conformance](https://github.com/vitnify/conformance):** a language-agnostic corpus so any implementation can be held to the spec.
- 🔐 A **Verification Authority** service + multi-tenant platform behind it (FastAPI · ed25519 · Postgres).

```bash
pip install vitnify        # Python SDK
cargo add vitni-tensor     # the deterministic engine
```

---

### 🧭 How I got here

I've been hunting threats my whole career, just in different domains. As a combat engineer, I cleared mines and IEDs off the roads and hunted the enemy on recon patrols. As an Air Defense Artillery officer, I tracked incoming aircraft and missiles. Cyber ran alongside all of it: app security, CTFs, and constant training while in uniform, then full-time threat hunting and incident response (CISSP). Same instinct every time: find the thing that shouldn't be there. Now I build the tools that make an AI's run something you can verify, not just trust.

### 🛠️ Stack

`Rust` · `Python` · `TypeScript` · LLM / GGUF / quantization · cryptography (ed25519, BLAKE3, Merkle) · AI-agent &amp; MCP security · deterministic / reproducible ML · AWS · PostgreSQL

<p align="center"><em>I'd rather build it than diagram it.</em></p>
