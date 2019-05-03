## Complex query

To do a search you can use the Complex Query Language (CQL), which is based on Lucene's syntax.

Free text search will look by default for:

Identifiers, names and synonyms of molecules (protein, gene, small molecule)
Identifiers, names and synonyms of complexes
Cross-references of complexes
Species
Search for groups of complexes by using the Gene Ontology. For example, GO:0016491 will search for all complexes annotated with "oxidoreductase activity" and all downstream child terms of this.

Narrow your initial search result by using the filters on the results page for:

- Species
- Molecule type
- Biological role

## Complex Query Language (CQL) fields

### Syntax highlight
```typescript
const language = 'typescript';
```

|Field Name          | Searches on   | Example  |
|--------------------|---------------|----------|
|`complex_id`          | right-aligned | [complex_id:CPX-2158](https://complex-portal.github.io/complex-portal-view/complex/search?query=complex_id:CPX-2158 "Search by complex ac")|
|`complex_alias`       | centered      |   $12  |
|`species`             | are neat      |    $1  |
|`complex_xref`        |               |        |
|`udate`               |               |        |
|`id`                  |               |        |
|`alias`               |               |        |
|`ptype`               |               |        |
|`pxref`               |               |        |
|`stc`                |               |        |
|`pbiorole`           |               |        |
|`ftype`               |               |        |
|`source`              |               |        |
|`number_participants` |               | [number_participants:3](https://complex-portal.github.io/complex-portal-view/complex/search?query=number_participants:3) |


### Lists
1. Ordered list
2. Another bullet point
  - Unordered list
  - Another unordered bullet point

### Blockquote
> Blockquote to the max!!!
