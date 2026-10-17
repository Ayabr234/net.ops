# net.ops

**An open-source, self-deployable, publicly funded hosting platform.**

net.ops aims to make web hosting public infrastructure: a system that any community, university, or cooperative can run for themselves, funded transparently by the people who use it rather than sold at a markup.

> **Status: early stage.** The project is in the research and design phase. Nothing here is production-ready yet, and everything under "Planned" is a goal, not a shipped feature.

---

## Why net.ops

Web hosting is concentrated among a small number of commercial providers. Individuals, communities, and small organisations depend on them for pricing, uptime, and policy decisions. There is no widely adopted open alternative that a group can deploy and operate on its own.

net.ops is an attempt to build that alternative by studying how the web ecosystem works end to end and turning it into an open, reproducible system.

## Goals

- **Study the web ecosystem:** DNS, routing, TLS, web servers, storage, isolation, orchestration, billing, and abuse handling.
- **Open architecture:** open specifications and reference components for every layer, reusing proven open-source tools wherever possible.
- **Self-deployable:** anyone can stand up their own hosting provider from the same codebase using only the documentation.
- **Publicly funded:** transparent resource accounting and support for donations, grants, and sponsorships.
- **Community governed:** open license, open specs, no vendor lock-in.

## Planned features

- Multi-tenant hosting for static and dynamic sites
- Domain and DNS management
- Automatic TLS certificate issuance and renewal
- Deployment via Git push, upload, or container image
- User dashboard and operator admin panel
- Per-tenant resource usage tracking
- Backups and restores
- Abuse reporting and takedown workflow

## Proposed stack (subject to change)

| Layer | Candidates |
|---|---|
| Reverse proxy / TLS | Caddy |
| Isolation | Docker or Podman |
| Private networking | WireGuard |
| Database | PostgreSQL |
| Provisioning | Ansible |
| Monitoring | Prometheus, Grafana |
| Backups | restic |

## Roadmap

Progress is gated by evidence rather than dates. Each phase must pass its test before the next begins.

1. **Define:** pick one user and one problem; validate with real people.
2. **Research:** map each layer of the web stack and choose existing components.
3. **Architecture:** write the specification.
4. **Prototype:** a single node serving isolated tenants, deployable by a third party from docs alone.
5. **Pilot:** a small group of real users; track uptime, cost per site, and support load.
6. **Funding and governance:** funding model, legal entity, license, abuse policy.
7. **Scale:** a second independent operator, then evaluate federation.

## Getting started

Installation and deployment instructions will be added once the prototype exists. For now, the best way to follow along is to watch this repository.

## Contributing

Contributions of every kind are welcome: research notes, architecture feedback, documentation, code, and real-world operator experience. Until the project has a contributor guide, please open an issue to discuss ideas before sending a pull request.

Particularly useful right now:
- Experience running community or non-profit hosting
- Knowledge of DNS, TLS, container isolation, or abuse handling
- Pointers to existing projects and funding sources

## Funding

net.ops is intended to be funded through a mix of grants, community contributions, and institutional sponsors. Funding details will be published openly as the model is developed.

## License

To be decided. An open-source license will be chosen before the first release.

## Contact

Open an issue on this repository to get in touch.
