![retromesh](https://github.com/user-attachments/assets/f3998540-970f-4189-9587-7f8c8c040d55)

RetroMesh is a community-driven darknet project restoring a 2010s‑style, corporate‑free social web. It emphasizes simple, human-driven discovery (no AI or recommendation algorithms) and provides access via a maintained fork of the Tor Browser. Privacy tools are available but optional — the project's primary focus is socialization and a corporate-free browsing layer reminiscent of the early decentralized web.

    WARNING: RetroMesh operates as a darknet overlay. Running or connecting to such a network can carry legal and security risks depending on your jurisdiction and how the network is used. Do not use RetroMesh for illegal activities. Use at your own risk.

Table of contents

    About
    Status
    Features
    Architecture
    Getting started
    Run a node
    Use the client
    Security & privacy
    Contributing
    License & legal

About

RetroMesh recreates the feel of the old web: small communities, curated link directories, forums, and personal pages — without AI‑driven feeds, commercial tracking, or platformized attention engines. The network prioritizes social interaction and community curation; privacy protections are provided as opt‑in features.
Status

This project is in early development. Many core components (including the first public build of the RetroMesh Tor Browser fork and production-ready node software) are still under development. Use the codebase for review, testing in sandboxes/VMs, and development contributions.

See the source code for Retromesh browser <a href="https://github.com/retromesh/client">here</a>

Features

    Darknet overlay accessed through a RetroMesh fork of Tor Browser.
    Human‑curated nodes and link directories (no algorithmic recommendations).
    Lightweight, text-first protocols for social posts, threads, and static pages.
    Simple discovery: peer lists, curated directories, and friend invites.
    Optional privacy tools: onion services, E2E messaging, ephemeral identities.
    Social-first: groups, events, and small-community circles.
    Minimal dependency on third-party analytics or corporate services.

Architecture

    Network layer: Tor‑based overlay. RetroMesh provides guidance and build instructions for a maintained Tor Browser fork configured for the network.
    Node software: lightweight daemon serving curated directories, relaying text content, and indexing human-curated lists.
    Client: RetroMesh fork of Tor Browser with UI integrations for node directories, peer lists, groups, and a basic composer.
    Protocols: small, human-readable, text-first protocols for posts, profiles, and threads — intentionally limited to avoid ranking/recommendation logic.
    Storage: optional local caches for pages, messages, and profiles; node operators may host voluntary public indexes.

Getting started

    Review local laws and the project warning. Operating or connecting to darknets may be restricted in some jurisdictions.
    Clone the repository: git clone https://github.com/Retromesh/Client.git
    Inspect directories:
        /client — Tor Browser fork code & build instructions (see /client/README.md)
        /node — node daemon code & config (see /node/README.md)
        /docs — design notes, protocol specs, and governance drafts
    Build and test in a sandboxed environment or VM before connecting to any live network.

Run a node

Minimum recommended specs: 1–2 CPU cores, 1–4 GB RAM, stable network.

    Read /node/README.md for dependencies and build steps.
    Copy config/example.yml → config.yml and edit:
        peers: curated peer list(s) you trust
        directories: the link directories you host
        moderation: local policy settings (optional)
    Start the daemon: ./retromesh-node --config config.yml
    Optionally register your node in community‑managed directories to aid discovery.

Use the client

    Build or download the RetroMesh Tor Browser fork following /client/README.md.
    Launch the browser; use integrated UI to browse node directories, send/accept friend invites, create/join groups, and post messages.
    Create a local identity (ephemeral identities recommended for casual use).

Security & privacy

    Privacy tools (onion services, E2E messaging, ephemeral identities) are opt‑in. Privacy is not required by default.
    Security recommendations:
        Test builds in a VM or sandbox before trusting them.
        Keep client and node software updated.
        Avoid sharing personally identifying information unless you accept the risks.
        Assume node operators may observe metadata unless privacy features are enabled.
    Threat model: community‑focused; not intended to guarantee anonymity against well‑resourced adversaries.

Contributing

    Read CONTRIBUTING.md and CODE_OF_CONDUCT.md.
    Fork the repo, create a feature branch, and open a PR. Include tests and documentation for code changes.
    We welcome code, documentation, curated directories, moderation tooling, UI/UX improvements, and security audits.

License & legal

RetroMesh is released under the GPLv3 License. See LICENSE for details.

RetroMesh is provided as‑is. The maintainers are not responsible for how the software is used. Connecting to or operating on darknet overlays may have legal consequences depending on jurisdiction. Understand and comply with local law.
