# Awesome-Personal-Knowledge-Management-PKM

# Top Personal Knowledge Management (PKM) Tools Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Local-First Data Ownership, Bidirectional Linking & Self-Hosted Sync*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Personal Knowledge Management (PKM)**. These tools help individuals capture, connect, and retrieve their own thinking — from daily notes and journaling to long-form research and networked thought — with a spectrum running from polished cloud workspaces to local-first Markdown files you own outright.

**Examples** include Obsidian, Logseq, SiYuan, AppFlowy, TriliumNext, Anytype, Notion, Roam Research, Tana, and Capacities (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, plain-text portability, and transparent data models — ideal for researchers, writers, and developers who want their second brain to outlive any vendor's pricing page.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Notion](https://www.notion.com/)**  
  **The reference all-in-one workspace** where pages and databases are the same primitive. Relations, rollups, and every view are polished. **Free for individuals**; Plus at **$10/member/month** (annual) . **Cloud-only** with limited offline mode. **Best for users wanting the most polished database-plus-notes experience** and willing to accept cloud dependency.

- **[Roam Research](https://roamresearch.com/)**  
  **The original networked-thought tool** that popularized bidirectional links and daily notes. **Commercial SaaS** with an annual subscription. **Best for academics and nonlinear thinkers** who want the graph-first methodology Roam pioneered [citation:11].

- **[Tana](https://tana.inc/)**  
  **Structured daily capture with a knowledge-graph workflow.** **Best for users wanting typed nodes and powerful Supertags** inside a cloud workspace [citation:14].

- **[Capacities](https://capacities.io/)**  
  **Polished, calm single-player PKM** with object-based organization. **Best for individuals wanting a beautiful, low-maintenance second brain** without local-file management [citation:14].

## Open-Source GitHub Projects

- **[SiYuan](https://github.com/siyuan-note/siyuan)**  
  **The privacy-first, self-hosted block-based PKM** — AGPL-3.0 licensed. **Local-first with optional cloud sync**; stores data in its own block structure rather than plain Markdown, enabling fine-grained block references and a native PDF annotation workflow . **Trade-offs**: **the granular "block-level" architecture imposes noticeable cognitive overhead for quick daily capture and continuous prose writing** [citation:7]. **Multi-device sync relies on paid official subscriptions or paying extra to unlock S3/WebDAV sync** with your own storage [citation:7]. **Best for users wanting a deeply structured, self-hosted PKM** with Chinese-language optimization and low configuration cost [citation:11].

- **[Logseq](https://github.com/logseq/logseq)**  
  **The open-source outliner-first PKM** — AGPL-3.0 licensed, local-first. **Every line is a block, referenceable from anywhere**; **journal workflow built in** for daily capture; **graph view** shows the web of connections across all notes . **Plain Markdown (or Org-mode) files on disk** for maximum AI compatibility and portability [citation:4]. **Trade-offs**: **no official self-hosted sync server** — relies on third-party Logseq Sync; **not a team/collaborative tool**, fundamentally personal and local-first; **learning curve** from the outliner paradigm [citation:4]. **Best for people who think in connections** and want a local-first, open-source alternative to Roam [citation:11].

- **[AppFlowy](https://github.com/AppFlowy-IO/AppFlowy)**  
  **The closest open-source Notion replacement** — AGPL-3.0, Rust and Flutter based. **Docs, databases (grid, kanban, calendar views), and notes in one app** [citation:2][citation:4]. **Local-first with self-hostable AppFlowy Cloud** (Docker Compose with API, auth, PostgreSQL, Redis, and S3-compatible storage) [citation:2]. **Trade-offs**: **self-hosted sync server setup is non-trivial**; **AI features are still maturing** and lag behind Notion AI; **fewer third-party integrations**; **performance on very large documents can be rough** [citation:4]. **Best for teams or individuals wanting a Notion-like interface** with full local ownership [citation:4].

- **[TriliumNext](https://github.com/TriliumNext/Notes)**  
  **The programmable hierarchical knowledge base** — AGPL-3.0, community fork of the archived Trilium Notes [citation:4][citation:6]. **JavaScript scripting inside notes** makes it a programmable knowledge system; **REST API (ETAPI)** for external integrations; **hierarchical tree organization** can go extremely deep; **relation maps** for visual linking; **self-hosted sync server** between desktop clients [citation:4]. **Storage**: **a single SQLite `document.db` file** — no PostgreSQL or Redis required, and **100,000 notes without performance issues** per official docs [citation:6]. **Features** include Markdown WYSIWYG, code notes with syntax highlighting, Excalidraw canvas, Mermaid diagrams, mind maps, geo maps, calendar, Kanban, tables, web clipper, and full-text search [citation:6]. **Trade-offs**: **UI looks dated** compared to AFFiNE or Outline; **not built for teams**, fundamentally single-user; **no managed cloud hosting** [citation:4]. **Best for power users and developers** wanting maximum flexibility and scripted automation [citation:4].

- **[Anytype](https://github.com/anytypeio/anytype-ts)**  
  **The encrypted, local-first object-based workspace** — **peer-to-peer sync** via the Any-Sync protocol with **no central server holding your data**; **local-first with offline-first architecture** [citation:4]. **Object-based data model** with typed objects and relations. **Note**: its client uses a **noncommercial source-available license** rather than a standard open-source license — organizations should review terms [citation:14]. **Best for privacy-maximalists** wanting encrypted local-first knowledge that syncs peer-to-peer.

- **[Alexandrie](https://github.com/Smaug6739/Alexandrie)**  
  **The self-hosted technical writing knowledge base** — **one-command Docker deployment** . **Extended CodeMirror 6 Markdown editor** with **LaTeX, custom containers, interactive checkboxes, native diagram rendering, and speech-to-text** . **Offline-first PWA** with full offline capabilities and sync . **Multi-tenant architecture** (Teams → Workspaces → Categories → Documents) with a **5-level access model** (None/Read/Write/Admin/Owner) . **OIDC SSO** and **S3-compatible storage** (RustFS, Garage, MinIO, AWS) . **Full-text indexing** with snippet highlights, **Ctrl+K command center**, and **Kanban boards** alongside documentation . **Best for technical teams** wanting a self-hosted Confluence/Notion alternative with LaTeX, diagrams, and enterprise auth [citation:15].

- **[Memos](https://github.com/usememos/memos)**  
  **The lightweight self-hosted memo hub** — MIT licensed, **single container backed by SQLite** [citation:2][citation:3]. **Twitter-style microblog for short, timestamped notes** — a personal changelog or daily log rather than a wiki . **Privacy-first** and one of the lightest tools available [citation:2]. **Best for quick daily capture** without the overhead of a full PKM system [citation:2].

- **[Flatnotes](https://github.com/dullage/flatnotes)**  
  **Self-hosted, database-less plain-text Markdown note-taking** — MIT licensed, Python/Vue [citation:3]. **Stores notes as plain files** with no database dependency. **Best for minimalists** wanting a simple, portable note archive.

- **[SilverBullet](https://github.com/silverbulletmd/silverbullet)**  
  **Self-hosted PWA for Markdown notes** — free and open-source [citation:3]. **Markdown-native with a browser-based editor**. **Best for users wanting a lightweight, self-hosted Markdown PKM** with PWA access.

- **[HedgeDoc](https://github.com/hedgedoc/hedgedoc)**  
  **Real-time collaborative Markdown notes** — community successor to CodiMD [citation:3]. **Best for collaborative Markdown editing** alongside personal knowledge capture.

### Additional Strong Open-Source Options

- **Zettlr** — Markdown editor for academics and researchers [citation:3].
- **Tangent Notes** — Local-first Markdown note-taking designed to let you write the way you think [citation:3].
- **Ephe** — Privacy-first, local-only Markdown paper for daily todos and thoughts [citation:3].
- **TiddlyWiki** — Self-contained JavaScript wiki for the browser, Node.js, and more [citation:3].

**Frameworks for building custom systems**: Combine **Logseq** for outliner-first networked thought with plain Markdown files, **SiYuan** for block-level references and PDF annotation in a self-hosted setup, **AppFlowy** for a Notion-style database workspace with local ownership, **TriliumNext** for programmable hierarchical knowledge with JavaScript scripting and a single SQLite file, and **Alexandrie** for self-hosted technical documentation with LaTeX and OIDC SSO — to build a PKM stack tailored to your thinking style, collaboration needs, and tolerance for operational overhead.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- PKM tools differ significantly in data model, sync architecture, and licensing. **Logseq has no official self-hosted sync server** and is fundamentally personal, not collaborative [citation:4]. **SiYuan's block-level architecture imposes cognitive overhead** for quick capture, and multi-device sync requires paid official subscriptions or extra fees to unlock S3/WebDAV [citation:7]. **AppFlowy's self-hosted sync is non-trivial** (multi-service Docker Compose) and its AI features lag behind Notion [citation:4]. **TriliumNext is single-user only** with a dated UI, but its JavaScript scripting and single-file SQLite storage make it uniquely programmable and portable [citation:4][citation:6]. **Anytype's client uses a noncommercial source-available license** — review before organizational use [citation:14]. **Obsidian's core is closed-source** despite its local-file model, and collaboration is weak [citation:11].
- Self-hosted open-source solutions require proper backup strategies (SQLite file for TriliumNext, PostgreSQL for AppFlowy), TLS configuration, and sync conflict monitoring.

---

**Made for researchers, writers, developers, and anyone building a second brain they can own and control.**
Let's make personal knowledge management more open, local-first, and data-sovereign.
