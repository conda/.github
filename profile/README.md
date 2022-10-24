[conda-org]: https://github.com/conda
[conda-incubator-org]: https://github.com/conda-incubator
[conda-archive-org]: https://github.com/conda-archive

[governance]: https://github.com/conda-incubator/governance
[coc]: https://github.com/conda-incubator/governance/blob/main/CODE_OF_CONDUCT.md#the-short-version
[ceps]: https://github.com/conda-incubator/ceps
[discourse]: https://conda.discourse.group/
[twitter]: https://twitter.com/condaproject

[transferring]: https://github.com/conda-incubator/governance#incorporate-a-software-project-into-the-main-conda-organization

[conda]: https://github.com/conda/conda
[conda-build]: https://github.com/conda/conda-build

# The conda Organization
Conda is an open-source organization and the community behind the [conda][conda] package manager.

The conda community is composed of three organizations here on GitHub:
- [conda][conda-org]: where officially supported projects live
- [conda-incubator][conda-incubator-org]: where community incubated projects live
- [conda-archive][conda-archive-org]: where inactive and archived projects live

The flowchart below explains how projects move within these organizations:

```mermaid
flowchart LR
    %% nodes
    community(Community):::community
    incubator(conda-incubator):::github
    conda(conda):::github
    archive(conda-archive):::github

    %% graph
    community-- invitation -->incubator
    incubator-- incorporation -->conda
    %% incubator-- inactive -->archive
    %% incubator-- unassociated -->community
    conda-- inactive -->archive
    %% conda-- dissolved -->incubator
    %% archive-- revived -->incubator

    %% style
    classDef community fill:#a5e8c1,stroke:#114226,stroke-width:2,stroke-dasharray: 5 5
    classDef github fill:#24292f,stroke:none,color:#fff
```

> **Note**
> Projects may also be directly added to the conda organization upon request to the
> steering council. For more details, please read [Incorporate a Software Project into the main conda Organization][transferring].

### Important Repositories

- [conda][conda]
- [conda-build][conda-build]

### Important Community Places

- [Governance][governance]: outlines and defines how the conda community works
- [CEPs][ceps]: Conda Enhancement Proposals
- [Discourse][discourse]: conda community discussion forum
- [Twitter][twitter]: for the latest developments

---

All interactions within the conda Organization are governed by our [Code of Conduct][coc].
