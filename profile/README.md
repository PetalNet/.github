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
| Jellyfin | `jellyfin.petalcat.dev` | Media server |
| Authentik | `auth.petalcat.dev` | SSO / OIDC provider |
| Uptime Kuma | `kuma.petalcat.dev` | Uptime monitoring |
| bsky-pds | `bsky.petalcat.dev` | AT Protocol personal data server |
| CollegeMap | `college.petalcat.dev` | Campus map app |
| OpenWebUI | `webui.petalcat.dev` | Local LLM inference |

## Repos

| Repo | Visibility | Purpose |
|---|---|---|
| [matrix-bot](../matrix-bot) | public | Matrix relay bot (Rust) |
| [PetalPVE](../PetalPVE) | public | Proxmox / Home Assistant custom component |
| [ActionOneHass](../ActionOneHass) | public | Action1 Home Assistant integration |
| [hassblink](../hassblink) | public | blink(1) USB LED Home Assistant integration |

## Naming

Services and tooling follow The Good Place theme.
