# NEXUS AI LAB — Enterprise AI Developer Console & Multi-Model Playground

> **"One Workspace. Endless Intelligence."**

**NEXUS AI LAB** is a unified, production-grade AI developer console and multi-model experimentation workbench. Built entirely with a zero-dependency, self-contained single-file architecture (`index.html`), it consolidates ultra-fast LPU inference, cloud foundation gateways, private on-premise local models, prompt engineering blueprints, side-by-side benchmarking, and agent tooling into a single futuristic workspace.

---

## 🎨 Theme & Visual Identity

The design system implements a futuristic midnight-blue & electric-cyan developer aesthetic:

| Design Token | Hex Code | Purpose |
|---|---|---|
| **Canvas Background** | `#080D1B` | Deep midnight space |
| **Sidebar Background** | `#0D1629` | Structural navigation drawer |
| **Workspace Panels** | `#131F35` | Primary interaction containers |
| **Elevated Containers** | `#192740` | Headers, wells, and inputs |
| **Subtle Borders** | `#293B57` | Structural dividing lines |
| **Primary Accent** | `#22D3EE` | Electric cyan buttons, active states |
| **Secondary Accent** | `#6366F1` | Indigo badges, user turn indicators |
| **Violet Accent** | `#A78BFA` | Creative tags & tool highlights |
| **Success Indicator** | `#34D399` | Throughput tags, connected status |
| **Warning / Demo** | `#FBBF24` | Demo mode indicator, key optional |

---

## 🏛️ Application Architecture & Core Feature Matrix

### 1. 🖥️ Master Playground (Image 1 Foundation)

The primary workbench implements every capability from the master playground reference:

#### A. Top Navigation & Studio Sub-Tabs
- **Chat & Reasoning**: Default high-throughput streaming workbench with multi-model support.
- **Vision & Audio**: Multimodal perception inspector for Meta Llama 3.2 11B Vision and Whisper Large v3 Turbo audio transcription benchmarks (`~216x realtime`).
- **Agents & MCP Tools**: OpenAPI function registry and Model Context Protocol (MCP) server bindings with parameter schema validation.
- **Safety & Guardrails**: Content moderation scanner powered by Meta Llama Guard 3 8B and Prompt Guard 2 86M for prompt injection detection.
- **Batch & Service Tiers**: Token budget calculator with 50% discount asynchronous batch estimations and TSP vs GPU latency comparisons.
- **Header Actions**:
  - `<> View Code`: Generates live code snippets in **cURL**, **Python SDK**, **JavaScript (`fetch` streaming)**, and **Node.js**.
  - **Set API Key**: Connects provider credentials stored exclusively in browser local memory.
  - **+ New Session**: Resets active conversation turns and output buffers.
  - **💾 Save**: Persists active session snapshots into the sidebar.

#### B. Workspace Presets
One-click pre-configured prompts that adjust models, temperatures, and instructions:
- **Multi-Step Logic Proof**: `openai/gpt-oss-120b` reasoning chain with formal theorem verification.
- **TypeScript Performance Audit**: `qwen/qwen-2.5-coder-32b` async pipeline profiling with zero-allocation buffers.
- **Strict JSON Schema Output**: `meta-llama/llama-3.3-70b-versatile` RFC 8259 structured entity extraction.
- **Ultra-Fast Chat Agent**: `llama-3.1-8b-instant` microservice (~1,250 tok/s).

#### C. Comprehensive Model Fleet
- **Groq LPU**: `llama-3.1-8b-instant` (~1,250 tok/s), `meta-llama/llama-3.3-70b-versatile` (~280 tok/s), `openai/gpt-oss-120b` (~320 tok/s), `qwen/qwen-2.5-coder-32b` (~350 tok/s), `mistralai/mixtral-8x7b-32768` (~480 tok/s).
- **OpenAI Cloud**: `gpt-4o`, `gpt-4o-mini`, `o3-mini`.
- **Google Gemini**: `gemini-2.0-flash` (1M context), `gemini-1.5-pro` (2M context).
- **Anthropic**: `claude-3-7-sonnet`, `claude-3-5-haiku`.
- **OpenRouter**: Open-weights router gateway.
- **Local Server (Ollama / vLLM)**: Private air-gapped inference on `localhost:11434`.

#### D. System Prompt Editor
- Labeled `SYSTEM` with `Cached Prefix` indicator.
- Persona presets (*Software Architect*, *Executive Summarizer*, *Strict JSON Generator*).
- `Clear` and `Reset` buttons.

#### E. API Connection Banner
- Clearly displays `DEMO MODE` or `LIVE CONNECTED`.
- Switch toggle between **Live Mode** and **Demo Mode**.
- Link to connect BYOK credentials with zero server-side storage.

#### F. Assistant Output Panel
- Streaming responses with real-time markdown formatting and syntax-highlighted code blocks.
- **Real-time Telemetry**: Latency (TTFT ms), Token count, and Throughput speed (`tok/s`).
- One-click `📋 Copy Markdown` and `🔊 Speak` (Web Speech API).
- Error recovery with retry guidance.

#### G. User Prompt Composer
- Large multiline input supporting `Ctrl+Enter` / `Cmd+Enter` execution.
- Multi-turn conversation container (`+ User Turn`, `+ Assistant Turn`).
- Attachment control (`📎 Attachment`).
- Real-time character and token estimation counter.

#### H. Complete Parameters Panel
1. **Stream Toggle**: Enable or disable real-time token streaming.
2. **JSON Mode Toggle**: Enforces valid RFC 8259 structured JSON output.
3. **Temperature Slider**: Range 0.00 to 2.00 with live numerical display.
4. **Max Output Tokens**: Range 1 to 8192 with numeric input validation.
5. **Top P (Nucleus)**: Range 0.00 to 1.00.
6. **Stop Sequences**: Comma-separated stop tokens.
7. **Built-in Tools**: Toggleable *Browser Search* (Exa-powered) and *Code Interpreter* (Python sandbox).
8. **Custom Function Tools**: `+ Add Function` modal with JSON Schema parameter editor.
9. **MCP Servers**: `+ Add Server` modal for Model Context Protocol connections.
10. **Advanced Parameters**: Frequency Penalty, Presence Penalty, Deterministic Seed.

---

### 2. 📋 Prompt Library (Image 3 + Custom Creation)
- **Search & Filter**: Keyword search with category chips (`All`, `Development`, `Productivity`, `Creative`, `Education`, `Business`).
- **6 Production Blueprints**:
  1. *Coding Assistant* (TypeScript / Python)
  2. *Executive Summarizer* (PRDs & meeting briefs)
  3. *Narrative & Creative Fiction* (Cinematic scene construction)
  4. *Technical Explainer* (Feynman pedagogy)
  5. *Venture Strategy Review* (Moat & unit economic modeling)
  6. *Code Security Auditor* (OWASP Top 10 remediation)
- **Custom Prompts**: `+ Create Custom Prompt` modal allows saving, editing, and deleting custom prompt blueprints stored in `localStorage`.
- **One-Click Loading**: Clicking any card loads system instructions and user prompt directly into the active playground.

---

### 3. 🌐 Model Explorer (Image 4)
- Specification table detailing Model Spec, Primary Gateway, Context Window, Optimal Workload, Throughput Profile, and direct `[ Use in Playground ]` actions.

---

### 4. ⧉ Side-by-Side Model Comparison (Image 5)
- Simultaneous dual execution of **Candidate Model A** and **Candidate Model B** on a shared evaluation prompt.
- Independent streaming buffers, latency meters, and token counters.

---

### 5. 📖 Documentation & Production Architecture (Image 6)
- **System Handbook**:
  1. *Multi-Gateway Protocol*
  2. *Dual-Mode Execution (Live vs. Demo)*
  3. *Sampling Temperature vs. Nucleus Sampling*
  4. *Multi-Turn Threading*
  5. *Resilience & Exponential Backoff*
  6. *Zero-Trace Security Guarantee*

---

### 6. ⚙️ Settings & Credentials (Image 6)
- BYOK API key storage for Groq, OpenAI, Google Gemini, Anthropic, and custom local Ollama/vLLM endpoints.
- Client runtime telemetry displaying storage footprint and session persistence status.

---

## 🚀 Quick Start

### Option A: Open Directly in Browser
```bash
open index.html
```

### Option B: Local HTTP Server
```bash
python3 -m http.server 8000
# Visit: http://localhost:8000
```

---

## ✅ Acceptance Test Checklist

| Feature Item | Reference | Status |
|---|---|---|
| **Top Studio Tabs** (Chat, Vision, Agents, Safety, Batch) | Image 1 | ✅ Tested & Working |
| **Workspace Presets** (Logic, TS, JSON, Fast) | Image 1 | ✅ Tested & Working |
| **Model Fleet** (Groq, OpenAI, Gemini, Anthropic, Ollama) | Image 1 | ✅ Tested & Working |
| **System Prompt Editor** (Cached prefix, Persona presets, Clear/Reset) | Image 1 | ✅ Tested & Working |
| **API Connection Banner** (Live / Demo mode toggle, BYOK info) | Image 1 | ✅ Tested & Working |
| **Assistant Output** (Streaming, markdown, code copy, speech, latency/speed) | Image 1 | ✅ Tested & Working |
| **User Prompt Composer** (Multiline, Ctrl+Enter, multi-turn, attachments) | Image 1 | ✅ Tested & Working |
| **Complete Parameters** (Stream, JSON, Temp, MaxTokens, TopP, Tools, MCP) | Image 1 | ✅ Tested & Working |
| **Prompt Library** (6 Curated cards + Custom prompt creation/filtering) | Image 3 | ✅ Tested & Working |
| **Model Explorer** (Table, gateways, throughputs, Use in Playground) | Image 4 | ✅ Tested & Working |
| **Side-by-Side Comparison** (Parallel execution of Model A vs B) | Image 5 | ✅ Tested & Working |
| **Documentation Handbook** (6 architectural cards) | Image 6 | ✅ Tested & Working |
| **Settings & Credentials** (Zero-trace BYOK management & telemetry) | Image 6 | ✅ Tested & Working |
| **NEXUS AI LAB Branding** (Midnight-blue `#080D1B`, cyan `#22D3EE`, logo) | All Images | ✅ Tested & Working |

---

## 🔒 Security & Privacy Guarantee

- **Zero Server-Side Storage**: All API keys, prompt histories, and session records remain strictly on the client inside browser `localStorage`.
- **Direct Encrypted HTTPS**: Live inference requests communicate directly with provider APIs (`api.groq.com`, `api.openai.com`, `generativelanguage.googleapis.com`) with zero intermediary telemetry or reverse proxies.
