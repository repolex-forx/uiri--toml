# Repolex Knowledge Graph of uiri/toml

RDF knowledge graph data for [uiri/toml](https://github.com/uiri/toml), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download uiri/toml
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── blob
│   ├── 08e981ffacfac174eaa37b6b0ae2743189f7953f.nq.gz
│   ├── 1be202fb4af4dad730bc5c84e19952e795e89308.nq.gz
│   ├── 25d431d3d7a1d93c3d77fc8297c402f87da7d42c.nq.gz
│   ├── 2850335c059713094e2ef74addf9545298de34e6.nq.gz
│   ├── 47aaec175be944e6210ede448244dfcda60212f9.nq.gz
│   ├── 4b7b3ab5b60406b4243b6a0c4ff4814971f4ef7e.nq.gz
│   ├── 4d468dd48898c82c2e5d862f90d373f95b8f14c2.nq.gz
│   ├── 5038eb3e4f17a3706a10fc2085cb0cef0bc7ba7e.nq.gz
│   ├── 5f947789d1156ba78b8a6bd79a90bdcd32b89a88.nq.gz
│   ├── 79bfd37b3d970f6417d09ec9d0aa63dba29dd7d1.nq.gz
│   ├── 815afc0e761aff28cf37c4c79f55dab01e89bf82.nq.gz
│   ├── 8f4e1ac50eacceb04175bfc057f157378e6ec851.nq.gz
│   ├── 93c3c8ad262fb2a024dc08ea5fd44040efd5a7c7.nq.gz
│   ├── 983d3bcc489b28aa11c9b37d0aa17c8b1ae4dcb7.nq.gz
│   ├── 9c20c41a1b9bcdb641dc52865bce04ccdb8f046c.nq.gz
│   ├── 9f0b57d152dcb73ef021b7b795b7d13fec24a1c8.nq.gz
│   ├── b85d356e1673bc8b470748e06f58e19431edc4a4.nq.gz
│   ├── c1dd22a0e397f0b381c16740893206c00e5af6dc.nq.gz
│   ├── cd4040d89c22572a5111f9d315c7a614b34e1136.nq.gz
│   ├── dcae0e817e907ffeaa7fc80c1f6194d3f1ce9755.nq.gz
│   ├── e02135960ae60455bf7e77e0576f1ce7a0da0024.nq.gz
│   ├── e436b271b0517a3b5afc1009f4a05d3e91ff359b.nq.gz
│   ├── e656b42d7482a765c2c6410a3fe1e65082bcc410.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e9e2c4efb5561670a9e160626ea9c77344af83f8.nq.gz
│   ├── f0e44a89aeb9f9b622665d66d3fa31f230172b26.nq.gz
│   └── fa382f3dc7dd514cdc258f8d4d2ca6ad271e4225.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 4935f616ef78c35a968b2473e806d7049eba9af1.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

8 directories, 33 files
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

## Source repository

[uiri/toml](https://github.com/uiri/toml)

---
*Parsed on 2026-03-21 by [repolex](https://repolex.ai)*
