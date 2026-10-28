# Repolex Knowledge Graph of jupyterlab/hatch-nodejs-version

RDF knowledge graph data for [jupyterlab/hatch-nodejs-version](https://github.com/jupyterlab/hatch-nodejs-version), parsed by [repolex](https://repolex.ai).

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
rlex download jupyterlab/hatch-nodejs-version
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 81c4612da14dec4b260bc956225fa24ab62b377e
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 81c4612da14dec4b260bc956225fa24ab62b377e
│           └── chunk-001.nq.gz
├── blob
│   ├── 0e46fb4ae03e7356a56cbb65f697f62dd32c4639.nq.gz
│   ├── 12b2dc712cc5417f6c50db2336ab8e0ffbe6d9d6.nq.gz
│   ├── 60af4c5f16741c7c2fe17cdd9718ae5f6d56d8a4.nq.gz
│   ├── 67ecd988641591ea0ab8cda684d8ff78e9157810.nq.gz
│   ├── 725feab5ce652dc39f3f2c77b9fd3c90bf049c65.nq.gz
│   ├── 78cce1c803b9eaa37eed49cfe6c4032e18561409.nq.gz
│   ├── 8393a44e6ff26a8fea118567e6e7afe223f232a5.nq.gz
│   ├── 872f16de518bf6c0261651db30df18a6c724415e.nq.gz
│   ├── 8cae8f630abf12cbf622f575d889521bf9ddb772.nq.gz
│   ├── 8dd399ab55bce8a4a1ddfd0c98170f771f6e5c35.nq.gz
│   ├── 94fd8d84d89cf9eabdf67f5e757b6977e7aa5da4.nq.gz
│   ├── 97fd431e6bcabde7fed2a86baa1d3bcf92f9bc51.nq.gz
│   ├── 9cacb78e84734ba231a466f3e118a7c02f06853a.nq.gz
│   ├── a42858a250ba80c404ffa417c8d2499ebe542215.nq.gz
│   ├── a61c02f77cd98402db0e1d80434fe59cdc4a64bb.nq.gz
│   ├── b8ee1fcf09230ddcc633c9e61597bc87ce4e2921.nq.gz
│   ├── bc9abad97803bc5e52460c9c59970df73940dd87.nq.gz
│   ├── c1881060de286b6e65824cf42d336f09ad37ce7e.nq.gz
│   ├── c61455cae075b956a4c079d94429d5a8c6c06b5e.nq.gz
│   ├── d716c8cb3b427d9f454e5116d441bc49f84feda2.nq.gz
│   ├── e0c6b7b6d609419bb8c411638047dd1964a87216.nq.gz
│   ├── e0e097c5cf0c75f0bc57290eef7d911073b291e6.nq.gz
│   ├── eadc2027bd707ff46c24fa4a8b1e85e0f2365009.nq.gz
│   ├── ed9e5f7afdf67e830ea8663d5ff48d8191519bcc.nq.gz
│   └── f470312dc1d20e59c708dead24ed07f144d5352b.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 81c4612da14dec4b260bc956225fa24ab62b377e.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 33 files
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

[jupyterlab/hatch-nodejs-version](https://github.com/jupyterlab/hatch-nodejs-version)

---
*Parsed on 2026-10-28 by [repolex](https://repolex.ai)*
