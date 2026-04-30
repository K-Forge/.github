# K-Forge `.github` (public org meta-repo) · Agent Context

> Operational context and rules for AI agents working in this repository.

---

## K-Forge Ecosystem

K-Forge is a software development club at Fundación Universitaria Konrad Lorenz (FUKL), Bogotá, founded by Brian Vargas (@13rianVargas).

| Project | Repo | Description |
|---------|------|-------------|
| **K-Forge `.github`** | `K-Forge/.github` | Public org meta-repo — you are here |
| K-Forge `.github-private` | `K-Forge/.github-private` | Members-only org meta-repo |
| K-Forge Website | `K-Forge/K-Forge` | Public landing page (Angular, Vercel) |
| KApp | `K-Forge/KApp` | University management platform (Spring Boot microservices) |
| TiendaQ | `K-Forge/TiendaQ` | University e-commerce system (Spring Boot + Angular) |
| Roastory | `K-Forge/Roastory` | Library-cafe management system (Node.js + MongoDB) |

---

## Repository Purpose

This is the **public meta-repository** for the K-Forge GitHub organization. GitHub uses this special `.github` repo to:

- Display the public organization profile at https://github.com/K-Forge (via `profile/README.md`).
- Provide community health files (`CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`) used as defaults across all K-Forge repos.
- Provide default issue/PR templates and workflows.

Everything that lives here is **public-facing** — visible to anyone visiting the K-Forge org page.

---

## Repository Structure

```text
.github/
├── profile/
│   ├── README.md              # K-Forge org public profile (rendered at github.com/K-Forge)
│   ├── CONTRIBUTORS.md        # Team members per project
│   └── assets/
│       ├── KForge-Purple-Logo.png
│       ├── project-banner.svg
│       └── public-banner.svg
├── .github/
│   ├── PULL_REQUEST_TEMPLATE.md   # Default PR template across all K-Forge repos
│   └── dependabot.yml             # Default dependabot config
├── CODEOWNERS                  # @13rianVargas owns everything by default
├── CODE_OF_CONDUCT.md          # Community code of conduct
├── CONTRIBUTING.md             # Git Flow + Conventional Commits + SemVer guide
└── SECURITY.md                 # Vulnerability reporting policy
```

---

## Brand Identity

- **Primary color:** Purple `#8B5CF6` (matches K-Forge Website Tailwind token `violet-primary`).
- **Accent color:** Deep purple `#4C1D95`.
- **Typography:** Default GitHub markdown + Fira Code for code samples.
- **Visual motif:** `◈` diamond bullets for section headers.
- **Tone:** Professional, formal, no emojis except where already present in PR templates.

Brand consistency goal: every public surface (org profile, contribute docs, repo READMEs) uses the same purple palette and the same project list.

---

## Conventions (org-wide)

These conventions are documented here and apply across **all** K-Forge repos:

- **Commits:** Conventional Commits, English, lowercase, no scope, no final period.
- **Branches:** Git Flow — `main`, `develop`, `feature/*`, `bugfix/*`, `chore/*`, `test/*`, `release/*`, `hotfix/*`.
- **Versioning:** SemVer `MAJOR.MINOR.PATCH`. Cycle: alpha → beta → stable.
- **Documentation:** Spanish for community docs (CONTRIBUTING/CODE_OF_CONDUCT/SECURITY). No emojis in technical markdown except section bullets (`◈`).
- **Contact:** `kforge.dev@gmail.com` for all official communication.

---

## AI Agent Instructions

- This repo controls the **public face** of the K-Forge organization. Changes here are visible to everyone visiting `github.com/K-Forge`.
- **Maintain story consistency:** any project listed in `profile/README.md` must match the actual repo state and the same description used elsewhere (Brian's profile, private profile, individual repo READMEs).
- **Active projects:** K-Forge Web, KApp, TiendaQ, Roastory. Do not add or remove without explicit request.
- **Brand:** keep purple palette `#8B5CF6` / `#4C1D95`. Do not introduce other colors except for status badges (where light purple `#A78BFA` indicates dev role, etc.).
- **CONTRIBUTORS.md:** keep the project name `TiendaQ` (NOT `TiendaK`). Update team rosters only when explicitly informed.
- **Org-wide files:** changes to `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md` affect every K-Forge repo. Treat them as load-bearing.
- **No emojis** in technical markdown unless already present.
- **No automatic commits.** Present changes for review first.
- **Documentation language:** Spanish for community docs.
