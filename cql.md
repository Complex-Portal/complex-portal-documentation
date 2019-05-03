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
|`complex_id`          | Complex identifier(s) | [complex_id:CPX-2158](https://complex-portal.github.io/complex-portal-view/complex/search?query=complex_id:CPX-2158 "Search by complex ac")|
|`complex_alias`       | Complex alias(es)      | [complex_alias:&quot;coenzyme Q-cytochrome c reductase&quot;]|
|`species`             | Complex Tax ID     |[species:9606](https://complex-portal.github.io/complex-portal-view/complex/search?query=species:9606)|
|`complex_xref`        | Complex xref(s)              | [complex_xref:15210332](https://complex-portal.github.io/complex-portal-view/complex/search?query=complex_xref:15210332)       |
|`udate`               | Last update of the interaction              | [udate:\[20110607 TO 20120906\]](https://complex-portal.github.io/complex-portal-view/complex/search?query=udate:[20110607 TO 20120906])      |
|`id`                  | Interactor identifier(s)               |  [id:P38326](https://complex-portal.github.io/complex-portal-view/complex/search?query=id:P38326)      |
|`alias`               | Interactor alias(es)               | [alias:Cyclin](https://complex-portal.github.io/complex-portal-view/complex/search?query=alias:Cyclin)       |
|`ptype`               | Interactor type(s)              |[ptype:protein](https://complex-portal.github.io/complex-portal-view/complex/search?query=ptype:protein)|
|`pxref`               | Interactor xref(s)              |[pxref:GO:0031577](https://complex-portal.github.io/complex-portal-view/complex/search?query=pxref:GO:0031577)|
|`stc`                 | Boolean value to know if the Interactor has stoichiometry information|[stc:true](https://complex-portal.github.io/complex-portal-view/complex/search?query=stc:true)|
|`pbiorole`            | Biological role(s)              |[pbiorole:enzyme](https://complex-portal.github.io/complex-portal-view/complex/search?query=pbiorole:enzyme)|
|`ftype`               | Feature type(s)              |[ftype:&quot;binding region&quot;](https://complex-portal.github.io/complex-portal-view/complex/search?query=|ftype:&quot;binding region&quot;)
|`source`              | Source database(s)              |[source:intact](https://complex-portal.github.io/complex-portal-view/complex/search?query=source:intact)|
|`number_participants` | Number of participants              | [number_participants:3](https://complex-portal.github.io/complex-portal-view/complex/search?query=number_participants:3) |


### Lists
1. Ordered list
2. Another bullet point
  - Unordered list
  - Another unordered bullet point

### Blockquote
> Blockquote to the max!!!
