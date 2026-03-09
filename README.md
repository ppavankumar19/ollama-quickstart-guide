# Ollama Quickstart Guide — 2026 Edition

A complete, device-friendly HTML reference guide for installing and using Ollama to run local LLMs on Linux, macOS, and Windows. Also includes an interactive Claude Code study guide and a full model catalog.

**Live URL:** [https://ollama.19062002.xyz/](https://ollama.19062002.xyz/)

---

## Pages

| File | Description |
|---|---|
| `index.html` | Main Ollama setup and implementation guide |
| `cc-learning-guide.html` | Interactive Claude Code study guide — 14 lessons |
| `ollamacatalog.html` | Ollama Model Catalog — 2026 Edition, 16 model profiles |

---

## What's Covered — Ollama Guide (`index.html`)

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

## What's Covered — Claude Code Guide (`cc-learning-guide.html`)

| Lesson | Description |
|---|---|
| 01 | What is a Coding Assistant? |
| 02 | What is Claude Code? |
| 03 | How Tool Use Works |
| 04 | Claude Code in Action |
| 05 | Adding Context |
| 06 | Making Changes & Power Modes |
| 07 | Controlling Context |
| 08 | Custom Commands |
| 09 | MCP Servers |
| 10 | GitHub Integration |
| 11 | Hooks — Automating Quality |
| 12 | Gotchas Around Hooks |
| 13 | Useful Hooks — Real Examples |
| 14 | The Claude Code SDK |
| — | Quick Reference Cheat Sheet |

---

## Models Covered

- **Llama 3.2** (Meta AI) — 1B / 3B — General purpose
- **DeepSeek R1** (DeepSeek AI) — 8B / 14B — Chain-of-thought reasoning
- **Gemma 3** (Google) — 4B / 12B — Multimodal
- **Qwen 3** (Alibaba) — 7B / 14B / 32B — Multilingual
- **Mistral** (Mistral AI) — 7B — Fast & efficient

---

## Quick Start

```bash
# Install Ollama (Linux)
curl -fsSL https://ollama.com/install.sh | sh

# Pull and run your first model
ollama pull llama3.2:1b
ollama run llama3.2:1b
```

Visit `http://localhost:11434` to confirm Ollama is running.

---

## System Requirements

| Resource | Minimum | Recommended |
|---|---|---|
| RAM | 8 GB | 16 GB+ |
| Disk | 12 GB free | 50 GB+ |
| GPU (optional) | NVIDIA 6 GB VRAM | NVIDIA 8 GB+ / Apple M-series |

---

## Usage

Visit the live site at [https://ollama.19062002.xyz/](https://ollama.19062002.xyz/) or open `index.html` in any modern browser — no build step or server required.

```bash
# Open directly
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

---

## Features

### index.html
- **Custom Favicon:** Branding icon shown in the browser tab.
- **Custom Domain:** Hosted at `ollama.19062002.xyz`.
- **Neural Network BG Pattern:** Subtle animated dot-and-line SVG background across the full page.
- **Sticky Navbar:** Brand logo, section numbers, and active-state highlighting.
- **Mobile Friendly:** Hamburger menu for small screens; responsive at 768px and 480px breakpoints.
- **OS-specific Tabs:** Native Windows, Linux, and macOS instructions with tab-switching.
- **One-click Copy:** Copy-to-clipboard on all code examples.
- **Progressive:** Scroll progress bar and back-to-top button.
- **Accordions:** Collapsible sections — all closed by default, opens one at a time.
- **CTA Buttons:** Two hero-section link buttons — "Learn Claude Code →" and "Explore Ollama Catalog →" — with hover animation.

### ollamacatalog.html
- **Full Design System Match:** Shares the exact Warm Craft Editorial theme from `index.html` — same CSS variables (parchment `#F4EDE4`, forest green, amber), same fonts (Fraunces, Syne, Fira Code), same neural network background.
- **16 Model Profiles:** Individual cards for Llama 3.x, DeepSeek-R1/V3, Mistral, Mixtral, Gemma 3, Phi-4/3, Qwen3/2.5, CodeLlama, nomic-embed-text, and LLaVA.
- **Overview Table:** Sortable summary of all 16 models — version, release date, size range, and category chips.
- **Search & Filter:** Sticky controls bar with live text search and category filters (General, Code, Reasoning, Vision, Edge, Embedding). Count label on the left; search input and filter buttons right-aligned.
- **Count-up Animation:** Hero stats animate on scroll using `IntersectionObserver` — numeric values count up with ease-out cubic easing; parameter range (`270M→671B`) uses a sequential reveal.
- **Verify Section:** CLI commands with copy button and official source links for checking current model availability.
- **Home Button:** Topbar "← Home" link always visible, styled in the page's forest green topbar.
- **Back-to-Top Button:** Fixed bottom-right, appears after scrolling 500px — identical to `index.html`.
- **Vol. I · 2026 Edition:** Edition label in the topbar.

### cc-learning-guide.html
- **Neural Network BG Pattern:** Same dot-and-line SVG pattern as `index.html`, adapted to the page's warm parchment palette via a `body::before` / `body::after` layering system with correct z-index stacking.
- **Count-up Animation:** Hero stats animate on scroll-into-view using `IntersectionObserver` and `requestAnimationFrame`:
  - `14` counts up from 0 (integer, ease-out cubic, 1.6 s)
  - `3.9×` counts up from 0× (1 decimal place)
  - `∞` scales in with a spring fade after a 400 ms delay
- **Back to Ollama Guide Button:** Topbar link (← Ollama Guide) always visible, styled to match the page's accent system.
- **14-Lesson Curriculum:** Structured lessons with step flows, analogy boxes, callouts, code blocks, tables, and interactive progress-check items.
- **Quick Reference Cheat Sheet:** Keyboard shortcuts, slash commands, prompt symbols, and hook exit codes in a grid layout.
- **Scroll Progress Bar:** Fixed bar at top shows reading progress.
- **Lesson Reveal Animation:** Each lesson fades and slides in on scroll via `IntersectionObserver`.
- **Checkboxes:** Interactive understanding-check items that mark themselves as done.
- **Back to Top Button:** Fixed bottom-right, appears after scrolling 500px.
- **Mobile Friendly:** Responsive at 640px and 480px — nav hides, grids collapse, font sizes scale down, touch targets are maintained.

---

## Cross-page Navigation

All three pages are linked to each other:

| From | Button | Goes to |
|---|---|---|
| `index.html` (hero) | "Also check out: Learn Claude Code →" | `cc-learning-guide.html` |
| `index.html` (hero) | "Explore: Ollama Catalog →" | `ollamacatalog.html` |
| `cc-learning-guide.html` (topbar) | "← Ollama Guide" | `index.html` |
| `ollamacatalog.html` (topbar) | "← Home" | `index.html` |
| `ollamacatalog.html` (footer) | "Back to Main Guide" | `index.html` |

---

## Changelog

### 2026 — Latest

- **Added `ollamacatalog.html`** — A full 16-model reference catalog covering every major Ollama model: Llama 3.x, DeepSeek-R1/V3, Mistral, Mixtral, Gemma 3, Phi-4/3, Qwen3/2.5, CodeLlama, nomic-embed-text, and LLaVA. Includes an overview table, individual model profile cards, and a CLI verify section.
- **Ollama Catalog theme** — Complete Warm Craft Editorial design system applied to `ollamacatalog.html`, matching `index.html` exactly: same CSS variables, fonts (Fraunces, Syne, Fira Code), neural network background, card styles, and chip system.
- **Count-up animation on catalog stats** — Hero stats animate on scroll via `IntersectionObserver` with ease-out cubic easing; `270M→671B` uses sequential text reveal.
- **Right-aligned controls bar on catalog** — Count label on left; search input and all filter buttons grouped and right-aligned.
- **Back-to-top button on catalog** — Fixed bottom-right button, identical to `index.html`, appears after 500px of scrolling.
- **Ollama Catalog CTA on `index.html`** — Added second hero CTA button "Explore Ollama Catalog →" alongside the Claude Code button; flex-wrap layout supports both buttons side by side.
- **Added `cc-learning-guide.html`** — A full 14-lesson interactive study guide for Claude Code, covering coding assistants, tool use, context management, custom commands, MCP servers, GitHub integration, hooks, and the SDK.
- **Neural Network BG Pattern on cc-learning-guide** — Added `body::before` (SVG tiled background) and `body::after` (semi-transparent overlay) matching the pattern used in `index.html`. Fixed z-index layering so all content (nav, main, footer) renders above the BG at z-index 1+.
- **Count-up Animation on cc-learning-guide** — Hero stats (14 Lessons, 3.9×, ∞) animate with an ease-out cubic counter triggered by IntersectionObserver when the hero enters the viewport.
- **Cross-page navigation** — All three pages now link to each other via topbar/hero CTA buttons.
- **Mobile Responsiveness improvements on cc-learning-guide** — Added 640px and 480px breakpoints: nav collapses, grids go single-column, font sizes scale, hero padding adjusts, touch targets are at least 44px, back button hides at 480px to prevent topbar overflow.
- **Updated Windows install** to use PowerShell one-liner (`irm | iex`).
- **Brightened terminal syntax colors** for better visibility on dark code blocks.
- **Custom Favicon** — Added `favicon.ico` with cache-busting query string and `shortcut icon` fallback.
- **Progress bar** — Fixed-top scroll progress indicator on both pages.

---

## Platform Support

Tested on:
- Windows 10/11 (Native)
- Ubuntu 20.04 / 22.04 / 24.04
- macOS 12+ (Intel & Apple Silicon)

---

## Resources

- [Ollama Official Site](https://ollama.com)
- [Ollama Model Library](https://ollama.com/library)
- [Ollama GitHub](https://github.com/ollama/ollama)
- [Ollama REST API Docs](https://github.com/ollama/ollama/blob/main/docs/api.md)
- [Python SDK](https://github.com/ollama/ollama-python)
- [JavaScript SDK](https://github.com/ollama/ollama-js)
- [Claude Code Docs](https://docs.anthropic.com)

---

*Built for developers — 2026 Edition*
