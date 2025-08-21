RetroMesh

![retromesh](https://github.com/user-attachments/assets/0a209671-93a0-434b-9662-f59645afbb97)

RetroMesh is a community-driven darknet project focused on restoring a 2010s-style, corporate-free web experience centered on socialization. The network emphasizes simple, human-driven discovery instead of AI or algorithmic recommendation. Access is provided via a maintained fork of the Tor Browser. Privacy tools are included and available, but use of them is optional — the primary goal is a social, anti-corporate browsing layer reminiscent of the early decentralized web.

    WARNING: RetroMesh operates as a darknet overlay. Running or connecting to such a network can carry legal and security risks depending on your jurisdiction and how the network is used. Do not use RetroMesh for illegal activities. Use at your own risk.

Table of Contents

    About
    Features
    Architecture
    Getting Started
    Running a Node
    Using the Network (Client)
    Security & Privacy
    Contributing
    License
    Disclaimer & Legal

About

RetroMesh recreates the feel of the old web: small communities, curated link directories, forums, and personal pages — without AI-driven feeds, commercial tracking, or platformized attention engines. The project targets social interaction and a corporate-free ecosystem; privacy protections are provided but optional.
Features

This project is currently in early developement stage, we still have a lot of things to work on before the first build of the Retromesh browser will be out.  

    Darknet overlay accessed through a forked Tor Browser.
    Human-curated nodes and link directories (no algorithmic recommendations).
    Lightweight protocols for text-first social spaces, static personal pages, and message boards.
    Simple discovery mechanisms (peer lists, curated directories, friend invites).
    Optional privacy tools (end-to-end messaging, onion services, ephemeral identities).
    Focus on socialization: groups, events, threads, and small-community circles.
    Minimal dependency on third-party analytics or corporate services.

Architecture

    Network layer: Tor-based overlay. RetroMesh uses a maintained fork of Tor Browser configured for the network’s routing and discovery conventions.
    Node software: lightweight node daemon to host curated directories, relay text content, and index human-curated lists.
    Client: the RetroMesh fork of Tor Browser with UI integrations for node directories, friend lists, groups, and a simple composer for posts/messages.
    Protocols: small, text-first protocols for posts, profiles, and group threads — intentionally limited to avoid algorithmic ranking.
    Storage: optional local storage for cached pages, messages, and user profiles. Nodes may offer voluntary public indexes curated by their operators.

Getting Started

    Read local laws and project warnings. Operating or connecting to darknets may be restricted in some jurisdictions.
    Clone this repository: git clone https://github.com//retromesh
    Review the code and build instructions for the Tor Browser fork and node software.
    Build and run in a sandboxed environment or VM when testing.

Running a Node

    Minimum requirements: modest CPU, 1–4 GB RAM, and stable network connectivity.
    Install dependencies (see /docs/INSTALL.md).
    Configure node settings in config.yml (peer lists, directories you wish to host, optional moderation policies).
    Start the node daemon: ./retromesh-node --config config.yml
    Register your node in community-curated directories to participate in discovery (optional).

Using the Network (Client)

    Use the RetroMesh fork of Tor Browser for network access. The fork includes UI elements for:
        Node directory browsing
        Friend invites and peer lists
        Group creation and thread browsing
    Launch the browser from the provided build or follow build instructions in /client/README.md.
    Create a local identity (ephemeral or persistent). Ephemeral identities are recommended for casual use.

Security & Privacy

    RetroMesh provides optional privacy tools (onion services, E2E messaging, ephemeral identities). Privacy is opt-in.
    The network intentionally avoids AI and algorithmic recommendation systems.
    Security recommendations:
        Use a sandbox/VM for running node software or client builds you don't fully trust.
        Keep the Tor Browser fork and node software updated.
        Avoid sharing personally identifying information unless you accept the risks.
        Assume nodes and peers can observe metadata unless you use privacy tools.
    Threat model: community-focused; not designed to provide guaranteed anonymity against well-resourced adversaries.

Contributing

    We welcome code, documentation, moderation tools, and curated directory contributions.
    Fork the repo, create a feature branch, and submit a PR. Follow the contribution guidelines in /CONTRIBUTING.md.
    Code of Conduct: respect the community and operate in ways that avoid enabling illegal activity. Abusive or illegal use that harms others is not supported.

License

RetroMesh is released under the MIT License. See LICENSE for details.
Disclaimer & Legal

RetroMesh is provided as-is. The maintainers are not responsible for how the software is used. Connecting to or operating parts of the darknet can have legal consequences. Understand and comply with local law.

design it / vibecode as a readme.md file
.
GPT-5 mini
RetroMesh

RetroMesh — a community-driven darknet focused on restoring a 2010s-style, corporate-free social web. No AI. No recommendation algorithms. Access via a maintained fork of the Tor Browser. Human-curated nodes, simple text-first protocols, and optional privacy tools.

    WARNING: RetroMesh is a darknet overlay. Running or connecting to such networks can carry legal and security risks depending on your jurisdiction and how the network is used. Do not use RetroMesh for illegal activity. Use at your own risk.

Table of contents

    About
    Key principles
    Features
    Architecture
    Quick start
    Run a node
    Use the client
    Security & privacy
    Contributing
    License & legal

About

RetroMesh recreates the small-community feel of the early decentralized web—forums, curated link directories, static personal pages, and simple social threads—without corporate platforms, tracking, or algorithmic feeds. The primary focus is socialization; privacy tools are available but optional.
Key principles

    Social-first: prioritize human interaction and community curation.
    Corporate-free: avoid reliance on corporate services and analytics.
    Simple protocols: text-first, intentionally limited feature set to prevent algorithmic ranking.
    Optional privacy: provide privacy tools (onion services, E2E messaging, ephemeral identities) but do not require them.
    Transparent moderation: nodes may opt into community moderation policies; enforcement is local.

Features

    Darknet overlay accessible via a forked Tor Browser.
    Human-curated node directories and peer lists (no AI recommendations).
    Lightweight node daemon for hosting directories, relays, and text content.
    Text-first social spaces: posts, threads, groups, events.
    Optional E2E messaging and ephemeral identities.
    Simple discovery: friend invites, peer lists, curated directories.
    Minimal client telemetry and no third-party trackers.

Architecture

    Network layer: Tor-based overlay. Access through a maintained RetroMesh fork of the Tor Browser configured for the network.
    Node: lightweight daemon that serves curated directories, relays messages, and indexes human-curated content.
    Client: RetroMesh Tor Browser fork with UI integrations for node directories, friend lists, group threads, and a composer.
    Protocols: small, human-readable text protocols for posts, profiles, and threads—designed to avoid ranking or recommendation logic.
    Storage: optional local caches. Node operators may host voluntary public indexes.

Quick start

    Read local laws and project warnings.
    Clone the repository: git clone https://github.com/retromesh/retromesh.git
    Inspect code and build instructions:
        /client/README.md — build instructions for the Tor Browser fork
        /node/README.md — node daemon build & config
    Build and test in a VM or sandbox before using on a production network.

    Download or build the RetroMesh Tor Browser fork (see /client/README.md).
    Launch the browser; use the integrated UI to:
        Browse node directories
        Send/accept friend invites
        Create or join groups and threads
        Post messages or host simple static pages
    Create a local identity (ephemeral recommended for casual use).

Security & privacy

    Privacy features are opt-in: onion services, optional E2E messaging, ephemeral/persistent identity choices.
    Recommendations:
        Test builds in sandbox/VM before trusting them.
        Keep client and node software updated.
        Avoid sharing personally-identifying information unless you accept the risk.
        Assume metadata may be visible to node operators unless you enable privacy features.
    Threat model: community-focused. Not designed to guarantee anonymity against nation-state or well-resourced adversaries.

RetroMesh is provided under the MIT License. See LICENSE for details.

RetroMesh is provided as-is. Maintainers are not responsible for how the software is used. Connecting to or operating parts of the darknet may have legal consequences in some jurisdictions. Understand and comply with local law.
