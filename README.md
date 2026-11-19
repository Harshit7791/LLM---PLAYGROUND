<div align="center">

# ⚡ NEXUS AI LAB
### *One Workspace. Endless Intelligence.*

**Enterprise AI Developer Console, Multi-Model Experimentation Workbench & Prompt Engineering Studio**

[![Status](https://img.shields.io/badge/Status-Production%20Ready-34D399?style=for-the-badge&logo=statuspage&logoColor=white)](https://github.com)
[![Architecture](https://img.shields.io/badge/Architecture-Single--File%20(index.html)-22D3EE?style=for-the-badge&logo=html5&logoColor=white)](https://github.com)
[![Dependencies](https://img.shields.io/badge/Dependencies-Zero%20(Vanilla%20ES6)-818CF8?style=for-the-badge&logo=javascript&logoColor=white)](https://github.com)
[![Inference](https://img.shields.io/badge/Inference-Ultra--Fast%20LPU%20%7C%20BYOK-FBBF24?style=for-the-badge&logo=speedtest&logoColor=black)](https://github.com)
[![Security](https://img.shields.io/badge/Security-Zero--Trace%20Client%20Sandbox-34D399?style=for-the-badge&logo=shield&logoColor=white)](https://github.com)
[![License](https://img.shields.io/badge/License-MIT-gray?style=for-the-badge)](LICENSE)

<br/>

[🚀 Quick Start](#-quick-start) • [🎛️ Core Capabilities](#️-core-capabilities) • [🚀 Engineering Innovations](#-engineering-architecture--core-innovations) • [📋 Prompt Blueprints](#-curated-prompt-library) • [⧉ Model Comparison](#-side-by-side-benchmarking) • [🔒 Zero-Trace Security](#-zero-trace-security-architecture)

---

</div>

## 📖 Overview

**NEXUS AI LAB** is a lightweight, high-performance developer console engineered for exploring, testing, and benchmarking production language models. Built entirely as a self-contained single-file web application (`index.html`), it pairs a futuristic midnight-navy developer interface with a dual-mode execution engine:

- **⚡ Live Streaming Mode**: Direct client-side SSE streaming to Groq LPUs, OpenAI, Google Gemini, Anthropic, OpenRouter, and local Ollama/vLLM servers.
- **🧪 Interactive Simulation Mode**: Deterministic, zero-credential simulation engine allowing instant offline UI evaluation without external API keys.

---

## 🎛️ Core Capabilities

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                                 NEXUS AI LAB                                    │
├──────────────┬───────────────────────────────────────────────────┬──────────────┤
│  WORKBENCH   │  STUDIO: [Chat] [Vision] [Agents] [Safety] [Batch]│  PARAMETERS  │
│  ──────────  │  ───────────────────────────────────────────────  │  ──────────  │
│  Playground  │  ⚡ Workspace Presets                             │  • Stream    │
│  Library     │  ⚙️ System Instructions (Cached Prefix)           │  • JSON Mode │
│  Explorer    │  💬 Multi-Turn User Prompt Composer               │  • Temp/TopP │
│  Compare     │  🤖 Streaming Assistant Output (TTFT, tok/s)      │  • Tools/MCP │
│  Docs / Set  │  📋 Copy • 🔊 Speech Synthesis • <> Code Export   │  • Penalties │
└──────────────┴───────────────────────────────────────────────────┴──────────────┘
```

### 1. 🖥️ Studio Workstations
- **💬 Chat & Reasoning**: Multi-turn dialogue with real-time token streaming, Markdown formatting, syntax-highlighted code with copy buttons, and Web Speech voice playback.
- **👁️ Vision & Audio**: Multimodal evaluation for Meta Llama 3.2 11B Vision and Whisper Large v3 Turbo transcription benchmarked at **~216x realtime**.
- **🤖 Agents & MCP Tools**: Integrated Model Context Protocol (MCP) server bindings and OpenAPI function registry with schema validation.
- **🛡️ Safety & Guardrails**: Live policy auditor testing prompts against MLCommons AI Safety standards via Meta Llama Guard 3 8B and Prompt Guard 2 86M.
- **📦 Batch & Service Tiers**: Interactive token budget calculator projecting 50% discounts for asynchronous batch queues vs. real-time Groq TSPs.

### 2. ⚡ Workspace Presets
Load end-to-end configured environments with a single click:
- **Multi-Step Logic Proof**: `openai/gpt-oss-120b` reasoning chain with formal mathematical verification.
- **TypeScript Performance Audit**: `qwen/qwen-2.5-coder-32b` profiling zero-allocation streaming pipelines.
- **Strict JSON Schema Output**: `meta-llama/llama-3.3-70b-versatile` RFC 8259 structured entity extraction.
- **Ultra-Fast Chat Agent**: `llama-3.1-8b-instant` microservice operating at **~1,250 tok/s**.

### 3. 🎚️ Comprehensive Parameter Studio
- **Stream Toggle**: Switch between real-time chunk streaming and single-payload completion.
- **JSON Mode**: Enforce RFC 8259 compliance at the inference runtime.
- **Temperature & Top P**: Granular sliders (0.00 to 2.00 / 0.00 to 1.00) with live telemetry.
- **Max Output Tokens & Stop Sequences**: Configure hard token caps and custom delimiters (`###`, `END`).
- **Built-in Tools**: Toggleable Exa-powered *Browser Search* and *Python 3 Code Interpreter*.
- **Custom Functions**: Register OpenAPI tools with custom JSON Schema parameter definitions.
- **MCP Servers**: Add stdio or SSE server connection endpoints.

---

## 🚀 Engineering Architecture & Core Innovations

NEXUS AI LAB is designed around five core engineering pillars to accelerate model evaluation from raw prompt prototyping to production deployment:

### 1. ⚡ Unified Multi-Engine Inference Pipeline
Rather than locking developers into a single proprietary ecosystem, NEXUS AI LAB normalizes divergent API protocols into an interoperable client-side dispatch layer:
- **Groq LPU Hardware Acceleration**: Harnesses deterministic Tensor Streaming Processors (TSPs) to deliver sustained throughput of **~1,250 tokens/sec** on lightweight models and sub-100ms Time-to-First-Token (TTFT) on complex 70B+ architectures.
- **Frontier Cloud Integration**: Direct, client-side bridges to OpenAI (GPT-4o, o3-mini), Anthropic (Claude 3.7 Sonnet), and Google Gemini (up to 2M context window).
- **Zero-Config Local Deployment**: Native integration with private on-premise clusters running **Ollama** or **vLLM** (`http://localhost:11434/v1`), enabling air-gapped private inference with zero cloud dependencies.

### 2. 📡 Real-Time SSE Chunking & Telemetry Engine
The application embeds a custom, high-speed Server-Sent Events (SSE) stream reader built directly on the browser's native `ReadableStream` API:
- **Instantaneous Delta Decoding**: Parses raw byte buffers on the fly without waiting for request completion or payload buffering.
- **Microsecond Precision Telemetry**: Continuously recalculates response latency, active generation throughput, and token counts.
- **Dynamic Stream Interruption**: Full `AbortController` cancellation loop that instantly terminates in-flight token streams at the hardware level.

### 3. 🛠️ Autonomous Agent Workstation & MCP Registry
Extends model capabilities beyond static text generation into active environment manipulation:
- **Model Context Protocol (MCP)**: Native stdio and SSE socket bindings connecting models directly to filesystem readers, search engines, and enterprise database drivers.
- **Runtime JSON Schema Validation**: Live tool parameter schema compiler allowing custom function registration directly from the UI.
- **Sandboxed Execution Bridges**: Integrated Exa web search and Python 3 evaluation environments.

### 4. 🛡️ Enterprise AI Safety & Injection Defense
Production prompt engineering demands rigorous risk screening. NEXUS AI LAB incorporates a dual-classifier moderation pipeline:
- **Meta Llama Guard 3 8B**: Evaluates incoming prompts and responses against MLCommons AI Safety standard taxonomies.
- **Prompt Guard 2 86M**: Real-time scanner trained specifically to detect privilege escalation, prompt injection attempts, and jailbreak vectors before inference execution.

### 5. 💾 Zero-Trace Client-Side Persistence
Every prompt, session history, and provider API key is managed with uncompromising privacy:
- **Strictly Local Memory**: Data never touches intermediate third-party proxy servers or analytics collectors.
- **One-Click Session Snapshots**: Persist, serialize, and export multi-turn conversations and parameters directly into portable JSON bundles.

---

## 📋 Curated Prompt Library

Filter blueprints by category or author custom prompts stored directly in `localStorage`:

- 💻 **Coding Assistant** (`Development`): Generates strictly-typed production code with Big-O complexity analysis.
- 📊 **Executive Summarizer** (`Productivity`): Distills meetings and PRDs into 3 core takeaways and prioritized action items.
- 🎭 **Narrative & Creative Fiction** (`Creative`): Cinematic scene building with atmospheric voice control.
- 🔬 **Technical Explainer** (`Education`): Explains algorithms via Feynman grounding metaphors.
- 📈 **Venture Strategy Review** (`Business`): Moat defensibility and unit economic evaluation.
- 🛡️ **Code Security Auditor** (`Development`): OWASP Top 10 detection with remediated drop-in patches.

---

## ⧉ Side-by-Side Benchmarking

Test candidate models simultaneously on identical prompts:
- **Parallel Dispatch**: Executes independent asynchronous requests across distinct provider gateways.
- **Real-Time Divergence Analysis**: Inspect reasoning differences, stylistic nuances, and token efficiency side-by-side.
- **Latency Telemetry**: Independent millisecond response latency and token count metrics.

---

## 💻 Implementation Code Export

Instantly export your active configuration to production code:

<details>
<summary><b>View Export Examples (cURL, Python, JavaScript, Node.js)</b></summary>

### cURL
```bash
curl https://api.groq.com/openai/v1/chat/completions \
  -H "Authorization: Bearer $GROQ_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "llama-3.1-8b-instant",
    "messages": [
      {"role": "system", "content": "You are a helpful assistant."},
      {"role": "user", "content": "Explain quantum superposition."}
    ],
    "temperature": 0.7,
    "stream": true
  }'
```

### Python SDK
```python
from groq import Groq

client = Groq()
completion = client.chat.completions.create(
    model="llama-3.1-8b-instant",
    messages=[
        {"role": "system", "content": "You are a helpful assistant."},
        {"role": "user", "content": "Explain quantum superposition."}
    ],
    temperature=0.7,
    stream=True
)

for chunk in completion:
    print(chunk.choices[0].delta.content or "", end="")
```

### JavaScript (`fetch` streaming)
```javascript
const response = await fetch("https://api.groq.com/openai/v1/chat/completions", {
  method: "POST",
  headers: {
    "Authorization": `Bearer ${process.env.GROQ_API_KEY}`,
    "Content-Type": "application/json"
  },
  body: JSON.stringify({
    model: "llama-3.1-8b-instant",
    messages: [
      { role: "system", content: "You are a helpful assistant." },
      { role: "user", content: "Explain quantum superposition." }
    ],
    temperature: 0.7,
    stream: true
  })
});

const reader = response.body.getReader();
const decoder = new TextDecoder();
while (true) {
  const { done, value } = await reader.read();
  if (done) break;
  console.log(decoder.decode(value));
}
```

</details>

---

## 🚀 Quick Start

### Method 1: Direct File Launch
Double-click `index.html` or run:
```bash
open index.html
```

### Method 2: Local HTTP Server (Recommended)
```bash
# Python 3
python3 -m http.server 8000

# Node.js (npx)
npx serve -l 8000 .
```
Navigate to **`http://localhost:8000`** in any modern web browser.

---

## 🔒 Zero-Trace Security Architecture

> [!IMPORTANT]
> **NEXUS AI LAB does not operate any intermediate proxy servers, tracking databases, or telemetry trackers.**

1. **Client-Side Sandbox**: All API credentials (Groq, OpenAI, Gemini, Anthropic) and saved session histories are stored exclusively in the browser's `localStorage`.
2. **Direct Browser-to-Provider HTTPS**: Streaming requests are dispatched directly from your browser to authenticated provider endpoints (`api.groq.com`, `api.openai.com`, `generativelanguage.googleapis.com`, or local `localhost:11434`).
3. **One-Click Purge**: Use the **Purge All Credentials** button in Settings to instantly wipe all tokens, keys, and cached prompts from your browser storage.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Description |
|---|---|
| <kbd>Ctrl</kbd> + <kbd>Enter</kbd> / <kbd>Cmd</kbd> + <kbd>Enter</kbd> | Execute prompt / trigger streaming generation |
| <kbd>Esc</kbd> | Dismiss open modal dialogs |
| <kbd>Cmd</kbd> + <kbd>?</kbd> | Open System Documentation Handbook |

---

## 📄 License
Open-source under the [MIT License](LICENSE). Built for AI researchers, prompt engineers, and production systems builders.
