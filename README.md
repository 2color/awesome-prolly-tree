# Awesome Prolly Tree [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

A Prolly Tree is a hybrid data structure that combines the features of B-trees and Merkle trees to provide both efficient data access and verifiable integrity. It is especially useful in distributed systems and peer-to-peer networks, allowing fast diffs and structural sharing.

## Contents

- [Implementations](#implementations)
  - [Go](#go)
  - [JavaScript](#javascript)
  - [Zig](#zig)
  - [TypeScript](#typescript)
  - [Rust](#rust)
- [Tools](#tools)
- [Learning Resources](#learning-resources)
- [Credits](#credits)


## Implementations

### Go

- https://github.com/dolthub/dolt
- https://github.com/attic-labs/noms
- https://github.com/RangerMauve/ipld-prolly-indexer/
- https://github.com/ABresting/Prolly-Tree-Waku-Message

### JavaScript

- https://github.com/mikeal/prolly-trees

### Zig

- https://github.com/canvasxyz/okra

### TypeScript

- https://github.com/tabcat/prollipop
- https://github.com/canvasxyz/okra-js

### Rust

- https://github.com/zhangfengcdt/prollytree

## Tools

- [KenCloud-Tech/prolly-tree-oracle](https://github.com/KenCloud-Tech/prolly-tree-oracle) - Enable smart contracts to create/read/update/delete to prolly trees.

## Learning Resources

- [Prolly Trees](https://www.dolthub.com/blog/2024-03-03-prolly-trees/) - Introduction to prolly-trees.
- [Merklizing the key/value store for fun and profit](https://joelgustafson.com/posts/2023-05-04/merklizing-the-key-value-store-for-fun-and-profit) - Content-defined merkle trees: A node is the first child of its parent if `u32(node.hash[0..4]) < (2^32 / Q)`.
- [Peer-to-peer ordered search indexes](https://0fps.net/2020/12/19/peer-to-peer-ordered-search-indexes/) - Peer-to-Peer Ordered Search Indexes and how Prolly Trees are used to implement them with comparison to Merkle Search Trees.
- [Efficient Diff on Prolly-trees](https://www.dolthub.com/blog/2020-06-16-efficient-diff-on-prolly-trees/) - Visual examples for prolly-tree diffs.
- [Probabilistic Merkle B-Trees in Noms](https://github.com/attic-labs/noms/blob/master/doc/intro.md#prolly-trees-probabilistic-b-trees) - One of the first design documents on prolly-trees from Noms.
- [Probabilistic Merkle B-Trees in Noms (slides)](https://docs.google.com/presentation/d/18zRxxI7plB0mJkhLPfo8KJ_f-tyIIPj9L4dZroyqEF0/edit#slide=id.g3615e39343_0_0) - Slides for the prolly-trees from Noms.
- [Prolly Tree PoC and technical writeup](https://github.com/waku-org/research/issues/78) - Custom implementation of prolly-tree with right side backbone.
- [Only Consider Keys](https://docs.dolthub.com/architecture/storage-engine/prolly-tree#only-consider-keys) - Only consider keys for chunk boundary, not keys + values.
- [Range-Based Set Reconciliation](https://logperiodic.com/rbsr.html) - Introduction to Range-Based Set Reconciliation with a mention of how it relates to Prolly Trees (Negantrophy section uses `[number, hash]` tuples as keys).
- [IPLD Prolly Tree Analysis](https://github.com/RangerMauve/blog.mauve.moe/pull/3) - Analysis of IPLD Prolly Trees.
- [Some notes and questions on Prolly Trees](https://github.com/attic-labs/noms/issues/3878)
- [Prolly Trees](https://jzhao.xyz/thoughts/Prolly-Trees) - An overview of Prolly Trees and how they compare to Merkle Search Trees.
- [Lab note #027 Breadcrumb to Prolly Trees](https://interjectedfuture.com/lab-notes/lab-note-027-breadcrumb-to-prolly-trees/) - A look at how Prolly Trees are used in Breadcrumb.

## Credits

- [Aaron Boodman](https://github.com/aboodman) - Inventor of the Prolly Tree.
- [Mikeal Rogers](https://github.com/mikeal) - Prolly Tree implementation in JavaScript.
- [tabcat](https://github.com/tabcat) - Creator of prollipop and originally compiled this list.
- [Tim Sehn](https://github.com/timsehn) - Prolly Tree implementation in Dolt.
- [Aaron Son](https://github.com/reltuk) - Prolly Tree implementation in Dolt.
- [Mauve Signweaver](https://github.com/RangerMauve) - IPLD Prolly Tree Analysis.
- [Joel Gustafson](https://joelgustafson.com/) - Zig implementation of Prolly Trees and author of blog posts.
- [Wil Chung](https://x.com/iamwil) - The Interjected Future Blog explaining many related concepts.
- [ABresting](https://github.com/ABresting) - Go implementation of prolly-tree with right side backbone.
- [Doug Hoyte](https://hoytech.com/about) - Author of blog post on range-based set reconciliation.
- [jchris](https://github.com/jchris) - Contributor to js prolly-tree implementation.
