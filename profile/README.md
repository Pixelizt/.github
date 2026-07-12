# Pixelizt

Design & growth studio. This org holds every Pixelizt system, product, and client workspace.

## How this org is organised

Repos are flat on GitHub, so we group them by **name prefix** and **topic** (filter the repo list by clicking a topic).

| Group | Topic | Repos | Access |
|---|---|---|---|
| 🔒 **Vault** | `vault` | `pixelizt` — secrets, playbooks, master handoff | Owners only |
| ⚙️ **Internal tools** | `internal` | `pixelizt-proposal`, `pixelizt-pricing`, `systemlab` | Team |
| 📦 **Product** | `product` | `leadlab-crm` — the LeadLab CRM | Team |
| 📐 **Template** | `template` | `client-template` — copied for every new client | Team |
| 👥 **Clients** | `client` | `client-<name>` — one repo per client | Team (+ that client, read-only, if needed) |

## Starting a new client

1. **Website:** open [extractor.pixelizt.com](https://extractor.pixelizt.com) → connect tokens → set **Create under: pixelizt** → name it `client-<name>` → Extract. The repo is born in this org with the site + a re-export workflow inside, deployed to Netlify.
2. **Strategy:** add the `client.md` / `seo-plan.md` / `CLAUDE.md` scaffold from **`client-template`** (or use “Use this template” for a fresh one).
3. Add the **`delivery`** team + the **`client`** topic. Fill in `client.md`.

## Access

- Team members → add to the **`@pixelizt/delivery`** team once; they get every working repo (not the vault).
- Clients → usually need no access; if one does, give read-only on their single `client-<name>` repo.

---
*Secrets live only in the private `pixelizt` vault — never in a client or public repo.*
