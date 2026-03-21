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
├── aggregate
│   ├── ast
│   │   ├── 3f637dba5f68db63d4b30967fedda51c82459471.nq.gz
│   │   ├── 4935f616ef78c35a968b2473e806d7049eba9af1.nq.gz
│   │   ├── a86fc1fbd650a19eba313c3f642c9e2c679dc8d6.nq.gz
│   │   ├── ab913af7e938d749c01ce88484ad8f7845817434.nq.gz
│   │   ├── b104386cb7a1d2f98a3751d5f17f2b9a903339e5.nq.gz
│   │   └── f730092955e574424fd92012f70e6b4283577687.nq.gz
│   ├── lsp
│   │   ├── 3f637dba5f68db63d4b30967fedda51c82459471.nq.gz
│   │   ├── 4935f616ef78c35a968b2473e806d7049eba9af1.nq.gz
│   │   ├── a86fc1fbd650a19eba313c3f642c9e2c679dc8d6.nq.gz
│   │   ├── ab913af7e938d749c01ce88484ad8f7845817434.nq.gz
│   │   ├── b104386cb7a1d2f98a3751d5f17f2b9a903339e5.nq.gz
│   │   └── f730092955e574424fd92012f70e6b4283577687.nq.gz
│   └── repolex
│       ├── 3f637dba5f68db63d4b30967fedda51c82459471.nq.gz
│       ├── 4935f616ef78c35a968b2473e806d7049eba9af1.nq.gz
│       ├── a86fc1fbd650a19eba313c3f642c9e2c679dc8d6.nq.gz
│       ├── ab913af7e938d749c01ce88484ad8f7845817434.nq.gz
│       ├── b104386cb7a1d2f98a3751d5f17f2b9a903339e5.nq.gz
│       └── f730092955e574424fd92012f70e6b4283577687.nq.gz
├── blob
│   ├── 02bbe2ae962a86ccc6aa0e3b184e2295d6ac6cc5.nq.gz
│   ├── 07ff1244004d17054bcffe0a7859a54f44f7cb9d.nq.gz
│   ├── 08e981ffacfac174eaa37b6b0ae2743189f7953f.nq.gz
│   ├── 0a7cc434b8573e703334264dbde103786514e3e2.nq.gz
│   ├── 0d26d1ee24e12b4c67bda3d0aae4a3212e666995.nq.gz
│   ├── 0f4292dc9485cf7f033307610eee0c11cb6450ae.nq.gz
│   ├── 11c4e0cbac010e4bcfa56d433c9a96621ecfbf86.nq.gz
│   ├── 1279723f3e41734f8b63165b67ef10fa7d7034fb.nq.gz
│   ├── 194a3583ef1f61b561e5adc12a72ebd3edb06c4f.nq.gz
│   ├── 1acc26fd618b8433f5b82de12caac1bbede22a81.nq.gz
│   ├── 1be202fb4af4dad730bc5c84e19952e795e89308.nq.gz
│   ├── 20a4406ff45e6d1dcfa3a2130eab940fd4261e1c.nq.gz
│   ├── 258ee42d97ec1b52b3d77d7ffacf25fe65efc21f.nq.gz
│   ├── 25d431d3d7a1d93c3d77fc8297c402f87da7d42c.nq.gz
│   ├── 2649d1ee1ceb34fd924bfbd1420495192a093738.nq.gz
│   ├── 2850335c059713094e2ef74addf9545298de34e6.nq.gz
│   ├── 32c245b4f2dc656de0e94e589b4c249307515f38.nq.gz
│   ├── 368dce1f5fcbff450d56b4f07729919ccdf3594a.nq.gz
│   ├── 3ec5b43afec1a0eeb33b361516639dda04b7d994.nq.gz
│   ├── 4769941f3c4a4cd12ec351f4cb8f091336498266.nq.gz
│   ├── 47aaec175be944e6210ede448244dfcda60212f9.nq.gz
│   ├── 48a465f97e385d6b1bfd6244b611c55b00a64e10.nq.gz
│   ├── 4b7b3ab5b60406b4243b6a0c4ff4814971f4ef7e.nq.gz
│   ├── 4d468dd48898c82c2e5d862f90d373f95b8f14c2.nq.gz
│   ├── 4d8db1a491d4ac52b396a7f6f78f1f674a9f8060.nq.gz
│   ├── 5010e3075e6b150fdfc0042ca4adb3d41335e08d.nq.gz
│   ├── 5038eb3e4f17a3706a10fc2085cb0cef0bc7ba7e.nq.gz
│   ├── 5f947789d1156ba78b8a6bd79a90bdcd32b89a88.nq.gz
│   ├── 62bca9a6afee3e612014ab66c0205fbc5c34dbf6.nq.gz
│   ├── 6f4f1591687a9eea55d75302ba002a4ccb4df40a.nq.gz
│   ├── 6fc48b22ed241d5bcce6fd1c42eb5a985ed80892.nq.gz
│   ├── 7719ac23a73c5b5fbe73c814229e594850ab9ae0.nq.gz
│   ├── 79bfd37b3d970f6417d09ec9d0aa63dba29dd7d1.nq.gz
│   ├── 7e13a0c36f42e5095fb43ae4c2361ace5db91888.nq.gz
│   ├── 815afc0e761aff28cf37c4c79f55dab01e89bf82.nq.gz
│   ├── 8162657a9bfe2642375f79e14cc219526ea1b910.nq.gz
│   ├── 8f4e1ac50eacceb04175bfc057f157378e6ec851.nq.gz
│   ├── 93c3c8ad262fb2a024dc08ea5fd44040efd5a7c7.nq.gz
│   ├── 94c20f449c9caa8d0e3794d37e7aea24ea22bfae.nq.gz
│   ├── 967d3dd15a3074775fc9f955ec84deb5ea85a4ca.nq.gz
│   ├── 983d3bcc489b28aa11c9b37d0aa17c8b1ae4dcb7.nq.gz
│   ├── 9c20c41a1b9bcdb641dc52865bce04ccdb8f046c.nq.gz
│   ├── 9f0b57d152dcb73ef021b7b795b7d13fec24a1c8.nq.gz
│   ├── aa514cc392e32e90f92218fda59365327e5fe2df.nq.gz
│   ├── ad130415f767fd5d8478a39c9b89ef659df33afb.nq.gz
│   ├── b65ae72ef40810f37371ecd90f58b73754755e93.nq.gz
│   ├── b85d356e1673bc8b470748e06f58e19431edc4a4.nq.gz
│   ├── bf17a72b62366870e2b73f2de8ff6c898105cf64.nq.gz
│   ├── bf20593a2647cb2cf0a858fb19734874867352ef.nq.gz
│   ├── bf400e97611327e2092f31ac16a4d620d3502b0a.nq.gz
│   ├── c05cbb18aea6df1f61a3781cf2df5ed3187befe4.nq.gz
│   ├── c1dd22a0e397f0b381c16740893206c00e5af6dc.nq.gz
│   ├── c1ea4441f8819bee81e24cdc7b9bae388f73cfe3.nq.gz
│   ├── c55b493cb7eba09b69455f5701925ea1089173e8.nq.gz
│   ├── cd4040d89c22572a5111f9d315c7a614b34e1136.nq.gz
│   ├── d9e557ed95d305bb3ac9d70bcb7ff59ebec1e652.nq.gz
│   ├── dcae0e817e907ffeaa7fc80c1f6194d3f1ce9755.nq.gz
│   ├── dd12eb37dc868e39155ad25b956ab05368bfb44c.nq.gz
│   ├── e02135960ae60455bf7e77e0576f1ce7a0da0024.nq.gz
│   ├── e436b271b0517a3b5afc1009f4a05d3e91ff359b.nq.gz
│   ├── e656b42d7482a765c2c6410a3fe1e65082bcc410.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e9e2c4efb5561670a9e160626ea9c77344af83f8.nq.gz
│   ├── ea1437def5621a3718b38877e10b54c238bd646d.nq.gz
│   ├── efb608589480c80408042bec0a61382c3d3a670b.nq.gz
│   ├── f0e44a89aeb9f9b622665d66d3fa31f230172b26.nq.gz
│   ├── f399c058aa54a28f2b4b618bef3f7d78ba985087.nq.gz
│   ├── f4895aadd896ee87befc03ac91056d85e56db2a0.nq.gz
│   ├── fa382f3dc7dd514cdc258f8d4d2ca6ad271e4225.nq.gz
│   ├── fbdef1c82e3659e0a8e240c7ac4db359a7d5bd10.nq.gz
│   ├── fd39468d8bff6b28a44ab4f7c54cce73715c527e.nq.gz
│   ├── fe37aead6e7acefd84731766cc3170e2b0d34c8b.nq.gz
│   └── ff9637fdf0b87bcc590ca14ee6aa8dfb4ff9894b.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   ├── 3f637dba5f68db63d4b30967fedda51c82459471.nq.gz
│   ├── 4935f616ef78c35a968b2473e806d7049eba9af1.nq.gz
│   ├── a86fc1fbd650a19eba313c3f642c9e2c679dc8d6.nq.gz
│   ├── ab913af7e938d749c01ce88484ad8f7845817434.nq.gz
│   ├── b104386cb7a1d2f98a3751d5f17f2b9a903339e5.nq.gz
│   └── f730092955e574424fd92012f70e6b4283577687.nq.gz
├── filetree
│   ├── 3f637dba5f68db63d4b30967fedda51c82459471.nq.gz
│   ├── 4935f616ef78c35a968b2473e806d7049eba9af1.nq.gz
│   ├── a240270b52930bbbd40bfb7316926e347d6ed642.nq.gz
│   ├── a86fc1fbd650a19eba313c3f642c9e2c679dc8d6.nq.gz
│   ├── ab913af7e938d749c01ce88484ad8f7845817434.nq.gz
│   ├── b104386cb7a1d2f98a3751d5f17f2b9a903339e5.nq.gz
│   └── f730092955e574424fd92012f70e6b4283577687.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 109 files
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
