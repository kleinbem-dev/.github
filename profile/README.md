<div align="center">
  <img src="https://raw.githubusercontent.com/kleinbem-dev/.github/main/profile/assets/logo.png" width="84" height="84" alt="kleinbem.dev logo" style="border-radius: 18px;" />
  <h1>kleinbem.dev</h1>
  <p><strong>Reproducible Systems · Local AI Execution · Developer Tooling</strong></p>

  <p>
    <a href="https://kleinbem.dev"><img src="https://img.shields.io/badge/website-kleinbem.dev-2563eb?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
    <a href="https://github.com/kleinbem"><img src="https://img.shields.io/badge/maintainer-@kleinbem-059669?style=for-the-badge&logo=github&logoColor=white" alt="Maintainer" /></a>
    <a href="https://nixos.org"><img src="https://img.shields.io/badge/ecosystem-NixOS-5277C3?style=for-the-badge&logo=nixos&logoColor=white" alt="NixOS" /></a>
  </p>
</div>

---

### 🌟 About

**kleinbem.dev** houses production-grade, open-source software tools and runtime platforms developed by [Martin Kleinberger](https://github.com/kleinbem). Each project here originated from real-world infrastructure, local AI orchestration, or developer workflows, engineered into reusable, standalone open-source products.

---

### 📦 Standalone Products & Projects

| Project | Tech Stack | Highlights |
| :--- | :--- | :--- |
| **[`cadre`](https://github.com/kleinbem-dev/cadre)** | Nix · Python · Ollama · Mesh-LLM | **Private AI teammates on your own compute.** Autonomous developer agents running on local hardware inference via Goose and custom execution runtimes. |
| **[`revue`](https://github.com/kleinbem-dev/revue)** | Rust · Svelte · Tailwind · Ollama | **Nix-native AI PR code review engine.** Automated code reviewer with smart multi-tier model fallback (Ollama, Claude, Gemini) and Forgejo/GitHub support. |
| **[`attic-ui`](https://github.com/kleinbem-dev/attic-ui)** | SvelteKit · TypeScript · Tailwind | **Modern web interface & store inspector for Attic.** Next-generation management portal for self-hosted Nix binary caches. |
| **[`nix-gantry`](https://github.com/kleinbem-dev/nix-gantry)** | NixOS · systemd-nspawn · Bash | **Zero-eval atomic container deployment.** Builds containers once in CI; target hosts fetch manifests and swap them atomically without local evaluation. |
| **[`nix-detour`](https://github.com/kleinbem-dev/nix-detour)** | Nix · Svelte · Nixpkgs | **Surgical Nixpkgs package detention.** Safely hold back broken packages from `nixos-unstable` or inject open PR fixes until upstream merges. |
| **[`foyer`](https://github.com/kleinbem-dev/foyer)** | SvelteKit · Tailwind · NixOS | **Next-gen homelab portal & service launchpad.** Lightweight, reactive application dashboard for multi-node self-hosted platforms. |

---

### 🏗 Architecture & Ecosystem

```mermaid
flowchart TD
    subgraph AI["🤖 Autonomous AI & Agents"]
        C["cadre<br/><i>Local compute agents</i>"]
        R["revue<br/><i>AI PR review engine</i>"]
    end

    subgraph Platform["⚡ Platform & Delivery"]
        G["nix-gantry<br/><i>Atomic container swap</i>"]
        D["nix-detour<br/><i>Upstream package safety</i>"]
        A["attic-ui<br/><i>Binary cache management</i>"]
    end

    subgraph Experience["🖥 Experience & Homelab"]
        F["foyer<br/><i>Service portal & dashboard</i>"]
    end

    AI --> Platform
    Platform --> Experience
```

---

### 📐 Engineering Values

- **Reproducibility First:** Built strictly on declarative infrastructure (Nix Flakes, OpenTofu, hermetic builds).
- **Local-First & Privacy-Conscious:** AI tools engineered for local, hardware-accelerated compute (CUDA, ROCm, Vulkan, Apple Silicon, Jetson).
- **High Performance:** Core systems and runtimes implemented in Rust; interfaces crafted with modern Svelte 5 / SvelteKit for near-instant reactivity.
- **Strict Quality Control:** Every repo runs declarative branch protection, sign-off rules, CodeRabbit automated reviews, and CI test pipelines.

---

### 🔗 Connect & Services

- **Founder & Maintainer:** [@kleinbem](https://github.com/kleinbem) (NixOS / nixpkgs package maintainer)
- **Consulting & Business:** [kleinbem.dev](https://kleinbem.dev)
- **Declarative Fleet Infrastructure:** [github.com/kleinbem](https://github.com/kleinbem)
- **Inquiries:** `martin.kleinberger@gmail.com`
