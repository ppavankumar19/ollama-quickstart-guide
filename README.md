# Ollama Quickstart Guide — 2026 Edition

A complete, device-friendly HTML reference guide for installing and using Ollama to run local LLMs on Linux, macOS, and Windows.

**Live URL:** [https://ollama.19062002.xyz/](https://ollama.19062002.xyz/)

## What's Covered

| Section | Description |
|---|---|
| 01 Prerequisites | System requirements, OS setup, essential tools |
| 02 Installation | Windows (Native), Linux, macOS installers |
| 03 Sign In | Ollama account setup and CLI authentication |
| 04 CLI Reference | All `ollama` commands + slash commands + env vars |
| 05 Models | Install & run Llama 3.2, DeepSeek R1, Gemma 3, Qwen 3, Mistral |
| 06 Testing | 3 CS prompts per model for benchmarking quality |
| 07 API & Python | REST API (cURL), Python SDK, JavaScript SDK examples |
| 08 Troubleshooting | Common errors and fixes |

## Models Covered

- **Llama 3.2** (Meta AI) — 1B / 3B — General purpose
- **DeepSeek R1** (DeepSeek AI) — 8B / 14B — Chain-of-thought reasoning
- **Gemma 3** (Google) — 4B / 12B — Multimodal
- **Qwen 3** (Alibaba) — 7B / 14B / 32B — Multilingual
- **Mistral** (Mistral AI) — 7B — Fast & efficient

## Quick Start

```bash
# Install Ollama (Linux)
curl -fsSL https://ollama.com/install.sh | sh

# Pull and run your first model
ollama pull llama3.2
ollama run llama3.2
```

Visit `http://localhost:11434` to confirm Ollama is running.

## System Requirements

| Resource | Minimum | Recommended |
|---|---|---|
| RAM | 8 GB | 16 GB+ |
| Disk | 12 GB free | 50 GB+ |
| GPU (optional) | NVIDIA 6 GB VRAM | NVIDIA 8 GB+ / Apple M-series |

## Usage

Visit the live site at [https://ollama.19062002.xyz/](https://ollama.19062002.xyz/) or open `index.html` in any modern browser — no build step or server required.

```bash
# Open directly
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

## Features

- **Custom Favicon:** Added branding icon to the browser tab.
- **Custom Domain:** Hosted at `ollama.19062002.xyz`.
- **Sticky Navbar:** Brand logo, section numbers, and active-state highlighting.
- **Mobile Friendly:** Hamburger menu for small screens.
- **OS-specific Tabs:** Native Windows, Linux, and macOS instructions.
- **One-click Copy:** Copy-to-clipboard on all code examples.
- **Progressive:** Scroll progress bar and back-to-top button.
- **Accordions:** Collapsible sections for dense content.

## Platform Support

Tested on:
- Windows 10/11 (Native)
- Ubuntu 20.04 / 22.04 / 24.04
- macOS 12+ (Intel & Apple Silicon)

## Resources

- [Ollama Official Site](https://ollama.com)
- [Ollama Model Library](https://ollama.com/library)
- [Ollama GitHub](https://github.com/ollama/ollama)
- [Ollama REST API Docs](https://github.com/ollama/ollama/blob/main/docs/api.md)
- [Python SDK](https://github.com/ollama/ollama-python)
- [JavaScript SDK](https://github.com/ollama/ollama-js)

---

*Built for developers — 2026 Edition*
