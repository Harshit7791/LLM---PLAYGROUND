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

[🚀 Quick Start](#-quick-start) • [🎛️ Core Capabilities](#️-core-capabilities) • [🌐 Model Fleet](#-unified-model-fleet) • [📋 Prompt Blueprints](#-curated-prompt-library) • [⧉ Model Comparison](#-side-by-side-benchmarking) • [🔒 Zero-Trace Security](#-zero-trace-security-architecture)

---

</div>

## 📖 Overview

**NEXUS AI LAB** is a lightweight, high-performance developer console engineered for exploring, testing, and benchmarking production language models. Built entirely as a self-contained single-file web application (`index.html`), it pairs a futuristic midnight-navy developer interface with a dual-mode execution engine:

- **⚡ Live Streaming Mode**: Direct client-side SSE streaming to Groq LPUs, OpenAI, Google Gemini, Anthropic, OpenRouter, and local Ollama/vLLM servers.
- **🧪 Interactive Simulation Mode**: Deterministic, zero-credential simulation engine allowing instant offline UI evaluation without external API keys.

---

## 🎨 Design System & Visual Palette

The console is crafted around an intentional, low-fatigue dark aesthetic tailored for continuous development sessions:

| Design Token | Hex Code | Visual Application |
|---|---|---|
| **Canvas Background** | `#080D1B` | Deep midnight canvas with subtle cosmic undertones |
| **Sidebar Drawer** | `#0D1629` | Structural navigation pane and persistent history |
| **Primary Panels** | `#131F35` | Workbench cards, parameter wells, and output viewports |
| **Elevated Containers** | `#192740` | Active headers, interactive buttons, and code blocks |
| **Structural Borders** | `#293B57` | High-contrast component framing |
| **Primary Accent** | `#22D3EE` | Electric cyan buttons, active nav tabs, slider thumbs |
| **Secondary Accent** | `#6366F1` | Indigo turn indicators and category badges |
| **Creative Accent** | `#A78BFA` | Violet tags and specialized tool calls |
| **Success Indicator** | `#34D399` | Ultra-fast throughput pills and active gateway status |
| **Warning / Demo** | `#FBBF24` | Key-optional indicator and simulated mode badges |

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

## 🌐 Unified Model Fleet

| Model Specification | Provider / Gateway | Context | Optimal Workload | Throughput Profile |
|---|---|---|---|---|
| **Llama 3.1 8B Instant** | Groq LPU | `128,000 tok` | Ultra-low latency microservices, instant agents | `⚡ ~1,250 tok/s` |
| **Llama 3.3 70B Versatile** | Groq LPU / OpenRouter | `128,000 tok` | Multihop logic, synthetic datasets, complex code | `⚡ ~280 tok/s` |
| **OpenAI GPT-OSS 120B** | Groq / Meta Compute | `128,000 tok` | Deep reasoning chains, theorem proofs, audits | `⚡ ~320 tok/s` |
| **Qwen 2.5 Coder 32B** | Groq LPU | `128,000 tok` | Full-stack refactoring, tests, vulnerabilities | `⚡ ~350 tok/s` |
| **Mixtral 8x7B Sparse MoE** | Groq / Mistral | `32,768 tok` | High-concurrency docs, multilingual pipelines | `⚡ ~480 tok/s` |
| **GPT-4o & GPT-4o Mini** | OpenAI Cloud | `128,000 tok` | Multimodal vision, complex tool orchestration | `~110 tok/s` |
| **Claude 3.7 Sonnet / Haiku** | Anthropic | `200,000 tok` | Nuanced prose, high-level software architecture | `~95 tok/s` |
| **Google Gemini 2.0 Flash** | Google AI Studio | `1,000,000 tok` | Massive repository context, video/audio reasoning | `⚡ ~240 tok/s` |
| **Local Models (Ollama / vLLM)** | Localhost (`:11434`) | `Dynamic` | Air-gapped private inference, sensitive records | `Local Hardware` |

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
