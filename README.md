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
    Clone this repository: git clone https://github.com/retromesh/retromesh.git 
    Review the code and build instructions for the Tor Browser fork and node software.
    Build and run in a sandboxed environment or VM when testing.

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

RetroMesh is released under the GPLv3 License. See LICENSE for details.
Disclaimer & Legal

RetroMesh is provided as-is. The maintainers are not responsible for how the software is used. Connecting to or operating parts of the darknet can have legal consequences. Understand and comply with local law.
