# Repolex Knowledge Graph of canonical/tls-certificates-operator

RDF knowledge graph data for [canonical/tls-certificates-operator](https://github.com/canonical/tls-certificates-operator), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download canonical/tls-certificates-operator
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 12f4ccde7cca1088cc642701c47a0a04160d9ce7
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 12f4ccde7cca1088cc642701c47a0a04160d9ce7
│           └── chunk-001.nq.gz
├── blob
│   ├── 0124f27d851dca57886af88a15fd715ac2be2ca6.nq.gz
│   ├── 0244a0782d0f483e26211d94996b7278656beca5.nq.gz
│   ├── 039b24ce608a6f98baa55da404674edc7912a810.nq.gz
│   ├── 0d787237e077dc4b6e69f69966285b7e2a209ec9.nq.gz
│   ├── 13af703428e23ce7d56cf7a1bc7061b64a8f6a18.nq.gz
│   ├── 19e4608cca2de3ef5347656ccb5d14e9f654fe22.nq.gz
│   ├── 1e8a8fb400b9bdf0dc725f127df8466a7b4f272a.nq.gz
│   ├── 262a2a57da10516b1343e5fdb8fcd222ffd99a24.nq.gz
│   ├── 30fcfbc86c0d7991d3e6d4ab197e65a19054f7d4.nq.gz
│   ├── 33a9aa1d3df00d73855c4ef37741e7e4e64269c3.nq.gz
│   ├── 4355e2afbfd8c3bc657adb853c36e993a9d71d07.nq.gz
│   ├── 4706b274a72e79f28da8210e819a9ca68dd8ef47.nq.gz
│   ├── 537a4bcb45096658d4cff78f31af0efe54757162.nq.gz
│   ├── 58b297cc1a58e9ce3a5750a4a67522ed974441ec.nq.gz
│   ├── 6ccd559eabeae93e4d23215fa450130fa9b37ace.nq.gz
│   ├── 6f5ba549bd0084ef1d8272964e28d7a3aa45d1bc.nq.gz
│   ├── 7d7367e937aba94db6855c479bf5b2c2149ef61f.nq.gz
│   ├── 7e9d50461abcf8053278e38c1eb264abc49fac0d.nq.gz
│   ├── 882a7d1b19caa64bd30e90f61997939ac5f66c2c.nq.gz
│   ├── 945fbc392a7ffb07256df8ba8809f4086748a4f1.nq.gz
│   ├── a4d73ec265c34b62213bbda833a2765e12f39c8c.nq.gz
│   ├── a8c1d19e9b863ff671e0247889508c7e7a0271c5.nq.gz
│   ├── ab22ecc7856790cbc3a203b1f7c51c76c01afce7.nq.gz
│   ├── ab3cb53c448552f1d17e467cb23db9843284851a.nq.gz
│   ├── bf0f2c48e2f5a8c868200bd56d36d94baf3b0f19.nq.gz
│   ├── bf3b1151cb4112c4de8b0591b05db925ceca4697.nq.gz
│   ├── c6aea43e2f93c0bf2f14ded7e08f11936a5d19ea.nq.gz
│   ├── c6cbb5bbbc07bff2a92713029600f82c8d901444.nq.gz
│   ├── d2fc5b80ed30b2e40e26116a506744c73e71dc07.nq.gz
│   ├── da38ad47055f3b7afa333b123515988cb887b4f0.nq.gz
│   ├── e6c487d640aac0eae26e777a5abeb0f8efe9f5a7.nq.gz
│   ├── e6cf2e45f2feb0a8b5442ffa2e6f9cf1bf102e8c.nq.gz
│   ├── ea9b6727679958d3f71d950d65dc247da09bf5d4.nq.gz
│   ├── eac33ee75c061ac095287a7d851b3e5627c3fa04.nq.gz
│   ├── f32ffc9e16f97a86e1bff6094526c9dff71b7f29.nq.gz
│   ├── fa6c4c4242ddde9c12673e4e2dbd1fe818b4c73e.nq.gz
│   ├── fa7e7720177c141f6c950c23ad8818d3bb042750.nq.gz
│   ├── fbbf4caee883abda797acaafd4b7be12a8101306.nq.gz
│   ├── fc3dc35c714419526f91de4020d8b805eb4440af.nq.gz
│   └── fcee0621e1c4086021af7a3a9971b12e2eab95e3.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 12f4ccde7cca1088cc642701c47a0a04160d9ce7.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[canonical/tls-certificates-operator](https://github.com/canonical/tls-certificates-operator)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
