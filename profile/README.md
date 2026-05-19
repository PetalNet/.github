# PetalNet

Personal homelab and self-hosted software ecosystem.

## Infrastructure

| Layer | What |
|---|---|
| Hypervisor | Proxmox VE |
| Docker host | Debian VM, Docker + containerd |
| Networking | UniFi |
| DNS / proxy | Cloudflare + Traefik (`*.petalcat.dev` wildcard) |

## Services

| Service | URL | Purpose |
|---|---|---|
| Synapse | `mx.petalcat.dev` | Matrix homeserver |
| Nextcloud | `cloud.petalcat.dev` | File sync + calendar |
| Jellyfin | `jelly.petalcat.dev` | Media server |
| Authentik | `auth.petalcat.dev` | SSO / OIDC provider |
| Uptime Kuma | `status.petalcat.dev` | Uptime monitoring |
| claude-corner | `claude.petalcat.dev` | Claude's structured output site |
| bsky-pds | `bsky.petalcat.dev` | AT Protocol personal data server |
| CollegeMap | `college.petalcat.dev` | Campus map app |
| ollama | internal | Local LLM inference |

## Repos

| Repo | Visibility | Purpose |
|---|---|---|
| [petalnet-infra](../petalnet-infra) | private | Docker Compose stacks, config, scripts |
| [homelab-docs](../homelab-docs) | private | Architecture docs, runbooks, network diagrams |
| [matrix-bot](../matrix-bot) | public | Matrix relay bot (Rust) |
| [PetalPVE](../PetalPVE) | public | Proxmox / Home Assistant custom component |
| [ActionOneHass](../ActionOneHass) | public | Action1 Home Assistant integration |
| [hassblink](../hassblink) | public | blink(1) USB LED Home Assistant integration |

## Naming

Services and tooling follow The Good Place theme.
