# kleinbem.dev

Open-source projects from Martin Kleinberger's infrastructure work, moved here once they are useful on their own.

## Projects

- [`nix-gantry`](https://github.com/kleinbem-dev/nix-gantry) — CI builds NixOS containers once; hosts fetch a manifest and swap them in atomically. No evaluation or building on the host.
- [`nix-detour`](https://github.com/kleinbem-dev/nix-detour) — single packages take a detour from your nixpkgs: hold one that broke in nixos-unstable, or run it from an open nixpkgs PR, until nixpkgs catches up.
- [`cadre`](https://github.com/kleinbem-dev/cadre) — private AI teammates on your own compute, powered by Goose over local inference (Ollama, MeshLLM).

More arrive as they get a license, a README written for strangers and CI: next, a Chrome extension that moves tabs into app windows.

The fleet these come from, NixOS hosts and OpenWrt routers as code, lives at [github.com/kleinbem](https://github.com/kleinbem).
