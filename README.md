# Repolex Knowledge Graph of adamchainz/django-minify-html

RDF knowledge graph data for [adamchainz/django-minify-html](https://github.com/adamchainz/django-minify-html), parsed by [repolex](https://repolex.ai).

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
rlex download adamchainz/django-minify-html
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── ec8c17abe8cf8e5acfcfb5228aaeb84b1e3eebeb
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── ec8c17abe8cf8e5acfcfb5228aaeb84b1e3eebeb
│           └── chunk-001.nq.gz
├── blob
│   ├── 12a61845155d30bc0d239cc6dd713ef5d4523d35.nq.gz
│   ├── 205ab9ad9df4ab629d1b7b8d8a72b41f44d8824c.nq.gz
│   ├── 22ddbb118475b52ce8ecba56d9ec45009923da58.nq.gz
│   ├── 27478df49a113ad187bae4575537f001fbab2bed.nq.gz
│   ├── 29784f81485cdbf547844f23d729c5fd3aaf2dcc.nq.gz
│   ├── 2a7f84f54867d02714727f82eef95d3be939d666.nq.gz
│   ├── 2bb4e6fc3cdf264607e18322872d79a1cf77f929.nq.gz
│   ├── 2d33605094d04c9a8065932a3269097dc879151d.nq.gz
│   ├── 3389e270132b51dd061bf1a6e94739bf741a66b3.nq.gz
│   ├── 3ba13e0cec6cbbfd462e9ebf529dd2093148cd69.nq.gz
│   ├── 40f4ac757715bb1a8c355eda9124141fdda3aeff.nq.gz
│   ├── 43cc74a5e777c3421a3ccdbeccc67d36db5234d8.nq.gz
│   ├── 621fa306edca291eb8617aa515dfc86902cc9caa.nq.gz
│   ├── 638524ab88345215437ebf54ec94fceb78e61172.nq.gz
│   ├── 7f1d007c01048570d774e58f46203d3e92056c39.nq.gz
│   ├── 8e62c9fa5583994ce153cb9644385a98c5f5c27e.nq.gz
│   ├── 8e9327fa08e130be92cdd610877eb91d322d45a6.nq.gz
│   ├── 8f80cdaf274bee1410ccbde69da90c5a8cf3611a.nq.gz
│   ├── 93acb639926ccf42e9a2f76f02419eeaf0405c3a.nq.gz
│   ├── 980521630a16a367483bd663f256a5925a2c516d.nq.gz
│   ├── b9d0a9c28e3b08ba6597be32a5a688031eccebb3.nq.gz
│   ├── d000126561019ebf4a23611d90f467b6b00cdabd.nq.gz
│   ├── e575748bc96fe92e4ddf4b5dd7e160ced92de29c.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── f7c509088c016fb272e03878d481b2e17982eab1.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── ec8c17abe8cf8e5acfcfb5228aaeb84b1e3eebeb.nq.gz
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

[adamchainz/django-minify-html](https://github.com/adamchainz/django-minify-html)

---
*Parsed on 2026-10-20 by [repolex](https://repolex.ai)*
