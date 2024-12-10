# awesome-prolly-tree

An awesome list for all things Prolly Trees.


## Implementations

| source | language |
| ------ | -------- |
| https://github.com/dolthub/dolt | go |
| https://github.com/mikeal/prolly-trees | JavaScript |
| https://github.com/canvasxyz/okra | Zig |
| https://github.com/tabcat/prollipop | TypeScript |
| https://github.com/attic-labs/noms | go |
| https://github.com/RangerMauve/ipld-prolly-indexer/ | go |

## Learning Resources:

- [Probabilistic Merkle B-Trees in Noms](https://github.com/attic-labs/noms/blob/master/doc/intro.md#prolly-trees-probabilistic-b-trees)
  - author: [Aaron Boodman](https://aaronboodman.com/)
  - [slides version]((https://docs.google.com/presentation/d/18zRxxI7plB0mJkhLPfo8KJ_f-tyIIPj9L4dZroyqEF0/edit#slide=id.g3615e39343_0_0))
  - 
 
- [Prolly Trees](https://www.dolthub.com/blog/2024-03-03-prolly-trees/)
  - author: [Tim Sehn](https://github.com/timsehn)
  - implementation: [dolt](https://github.com/dolthub/dolt)
  - note: great introduction to prolly-trees

- [Prolly Tree PoC and technical writeup](https://github.com/waku-org/research/issues/78)
  - author: [ABresting](https://github.com/ABresting)
  - implementation: [Prolly-tree-Waku-Message](https://github.com/ABresting/Prolly-Tree-Waku-Message)
  - note: Custom implementation of prolly-tree with right side backbone

- [Merklizing the key/value store for fun and profit](https://joelgustafson.com/posts/2023-05-04/merklizing-the-key-value-store-for-fun-and-profit)
  - author: [Joel Gustafson](https://joelgustafson.com/)
  - implementation: [okra-js](https://github.com/canvasxyz/okra-js/tree/main/packages/okra)
  - note: content-defined merkle trees: A node is the first child of its parent if u32(node.hash[0..4]) < (2^32 / Q).

- [Efficient Diff on Prolly-trees](https://www.dolthub.com/blog/2020-06-16-efficient-diff-on-prolly-trees/)
  - author: [Aaron Son](https://github.com/reltuk)
  - implementation: [dolt](https://github.com/dolthub/dolt)
  - note: excellent visual examples for prolly-tree diffs

- [Only Consider Keys](https://docs.dolthub.com/architecture/storage-engine/prolly-tree#only-consider-keys)
  - author: [Tim Sehn](https://github.com/timsehn)
  - implementation: [dolt](https://github.com/dolthub/dolt)
  - note: only consider keys for chunk boundary, not keys + values

- [Range-Based Set Reconciliation](https://logperiodic.com/rbsr.html)
  - author: [Doug Hoyte](https://hoytech.com/about)
  - note: Negantrophy section uses [number, hash] tuples as keys

- [IPLD Prolly Tree Analysis](https://github.com/RangerMauve/blog.mauve.moe/pull/3)
  - author: [Mauve Signweaver](https://github.com/RangerMauve)
 
- [Some notes and questions on Prolly Trees](https://github.com/attic-labs/noms/issues/3878)
  - authors: [Mikeal Rogers](https://github.com/mikeal) and [Aaron Boodman](https://github.com/aboodman)


## Credits

- [Aaron Boodman](https://github.com/aboodman) for inventing the Prolly Trees
- [tabcat](https://github.com/tabcat) for originally compiling this list of resources
