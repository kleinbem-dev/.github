# kleinbem

Personal infrastructure-as-code fleet: NixOS + OpenWrt, managed across ~16 independent repos.

## Start here

- [`kleinbem`](https://github.com/kleinbem/kleinbem) — fleet hub: `repos.nix` (the manifest of every repo below), fleet-wide `just` recipes, the dashboard tooling
- [`nix`](https://github.com/kleinbem/nix) — conductor for the NixOS side ([`nix-config`](https://github.com/kleinbem/nix-config) is where the actual hosts/modules live)
- [`openwrt`](https://github.com/kleinbem/openwrt) — conductor for the router side ([`openwrt-builder`](https://github.com/kleinbem/openwrt-builder), [`openwrt-config`](https://github.com/kleinbem/openwrt-config))

## How it's built

- **VCS:** [Jujutsu](https://jj-vc.github.io/jj/) (colocated with git), automated via [`jj-toolbox`](https://github.com/kleinbem/jj-toolbox)
- **Secrets:** sops + age, per-path scoped, in a dedicated encrypted repo
- **Deploys:** standalone NixOS containers built centrally, not evaluated per-host
- **IaC:** OpenTofu/Terraform for anything self-contained (GitHub org settings, Cloudflare, etc.)

Every repo is an independent peer with its own history and CI — none of this is a monorepo or git submodules.
