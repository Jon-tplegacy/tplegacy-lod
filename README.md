# tplegacy-lod

Linked Open Data dump of the [True Parents Legacy](https://tplegacy.net/) digital archive.

## What's here

| File | Description |
|---|---|
| `tplegacy.nt` | RDF dump in N-Triples format (auto-updated weekly) |
| `void.ttl` | VoID dataset description for LOD Cloud registration |
| `stats.json` | Triple and link counts (auto-updated) |

## Dataset

- **3,700+ passages** — sermons, speeches, prayers, and book excerpts
- **Authors:** Sun Myung Moon (1920–2012), Hak Ja Han Moon (1943–present)
- **Period:** 1946–2012
- **Language:** English
- **License:** [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)

## Linked Data links

| Target | Predicate | Count | Wikidata IDs |
|---|---|---|---|
| Wikidata — persons | `schema:sameAs` | ~3,400 | Q131433, Q493527 |
| Wikidata — organizations | `schema:sameAs` | 2 | Q217059, Q138757400 |
| Wikidata — content types | `schema:sameAs` | 5 | Q861911, Q40953, Q1441437, Q628996, Q334291 |
| n2t.net ARK resolver | `schema:sameAs` | ~3,700 | — |
| Creative Commons | `schema:license` | ~3,700 | — |

## How it's generated

A [GitHub Action](https://github.com/andresigdev/tplegacy-theme/actions) in the theme repo runs weekly:

1. Fetches all posts from Content API
2. Converts to RDF N-Triples (schema.org vocabulary)
3. Pushes `tplegacy.nt` and `stats.json` here

## LOD Cloud

This dataset is submitted to [lod-cloud.net](https://lod-cloud.net/) under the **Publications** domain.

- **NAAN:** 68749 (ARK persistent identifiers)
- **Wikidata:** [Q138757400](https://www.wikidata.org/wiki/Q138757400)
- **VoID:** [`void.ttl`](void.ttl)
