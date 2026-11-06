# Repolex Knowledge Graph of zopefoundation/zope.processlifetime

RDF knowledge graph data for [zopefoundation/zope.processlifetime](https://github.com/zopefoundation/zope.processlifetime), parsed by [repolex](https://repolex.ai).

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
rlex download zopefoundation/zope.processlifetime
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── d8906386d6c7bb2105f38c0e0ca891a107aa816c
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── d8906386d6c7bb2105f38c0e0ca891a107aa816c
│           └── chunk-001.nq.gz
├── blob
│   ├── 398ba5d57adc57ca1608c347d9ac797f5cca3478.nq.gz
│   ├── 40ed1c630632f6bb1079970613fd22c3e49f365b.nq.gz
│   ├── 4df306eb09b0b6be7e693ba9d75a61ae28c164d4.nq.gz
│   ├── 4fceededc076d99e16426f0d4707c9234ea622a2.nq.gz
│   ├── 5901d87d9fa692ef5d4f3dceef0fc277098f81a1.nq.gz
│   ├── 623fa469a6a921299e79918b06678a76f9042013.nq.gz
│   ├── 7aa4a014ea0dfe3f591bf1383a8bb10ce05e8b04.nq.gz
│   ├── 8848873cbeb3ef72d66aef8b481d5f4e8bcf1e47.nq.gz
│   ├── 99e416636146aff510c95b785fa889bd18953ff4.nq.gz
│   ├── 9f2e6a0586bc6507faa5369c4a09cb7e1c5d71fb.nq.gz
│   ├── af169da47955d09ae265391ba0ba292fbdad1ba1.nq.gz
│   ├── b44c7f73084e2574f696e5fd4f9aa96746a0a883.nq.gz
│   ├── b8581dd898cbb33e63961b4d181ff0ffbe5d03ee.nq.gz
│   ├── bdb19d36f52f9efdf0d50627645d0811ce3657c2.nq.gz
│   ├── c4c4d3a87e724384193c31271220bce6f89cab51.nq.gz
│   ├── ca517f4eb0cec1c691c0c2b54cd5eb85e906f11b.nq.gz
│   ├── cdabe12cdedc172595c7a53a1cfebe1bfae265b1.nq.gz
│   ├── d9a1005de525a99d7149ae38092c76b0d36dcff3.nq.gz
│   ├── d9e113ec685b92b018297dd2f200341d1fba01f9.nq.gz
│   ├── e184fd8f41cbc229060cf69967d916bf6e2ddf2a.nq.gz
│   ├── e1f9ad7b3b48377bfbfaa1b380c384ddea24060f.nq.gz
│   ├── e4b867329e05886a4818f86b117fca2102bc84bf.nq.gz
│   ├── ea786d2513859fc0e710566b2e9b5b8c9b28bfe8.nq.gz
│   ├── f4eb4ef03531cc8d542efa457d2880e2c8e3ec49.nq.gz
│   ├── f507feda73c43de02c9268ef502bc4c3a2ebf32d.nq.gz
│   └── f81cabf053fb4487bb3496afbc276556076bc3f2.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── d8906386d6c7bb2105f38c0e0ca891a107aa816c.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 34 files
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

[zopefoundation/zope.processlifetime](https://github.com/zopefoundation/zope.processlifetime)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
