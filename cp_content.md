## Data Content

### What can be described as a complex

A stable set of (two or more) interacting macromolecules such as proteins which can be co-purified by an acceptable method and have been shown to exist as an isolated, functional unit in vivo. Any interacting, integral non-protein molecules (e.g. small molecules, nucleic acids) may also be included.

### What should **NOT** be captured:

- Enzyme/substrate, receptor/ligand or any similar transient interactions unless these are a critical part of the complex assembly (e.g. PDGF receptors only become 'dimeric' when linked by the dimeric ligand forming a tetramer).
- Proteins associated in a pulldown/coimmunoprecipitation with no functional link or any evidence that this is a defined biological entity rather than a loose affinity complex.
- Any literature complex where the only evidence is based on genetic interaction data.
- Partial complexes


### Tricky cases we **DO** capture:

- Substrates or ligands if the enzyme or receptor complex only forms in their presence (see PDGF receptors above, e.g. CPX-2883).
- Homologous proteins, with the same functionality, which would be inferred based on homology of the genome-encoded components made primarily on functional conservation between the two systems to form a complex but for which no physical link has been demonstrated, e.g. proteins A and B have been shown to physically interact and form a functional complex, protein C is a homologue of protein B by sequence similarity and is know to have the same function as B but protein A-C interaction has not been demonstrated experimentally (e.g. SUMO - E1 ligase complexes: there is interaction evidence for binding with SUMO1 ([CPX-3042](https://www.ebi.ac.uk/complexportal/complex/CPX-3042)) but not with SUMO2 ([CPX-3044](https://www.ebi.ac.uk/complexportal/complex/CPX-3044))). These complexes are tagged with [ECO:0005546 biological system reconstruction evidence based on paralogy evidence used in manual assertion](https://www.ebi.ac.uk/ols/ontologies/eco/terms?iri=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FECO_0005546).
- Complexes which are generally assumed to exist but for which only partial experimental evidence exists (such as functional studies or ligand binding evidence from pharmacological experiments), e.g. [Muscle-type nicotinic acetylcholine receptor complex, alpha1-beta1-delta-gamma](https://www.ebi.ac.uk/complexportal/complex/CPX-2179). These complexes are tagged with [ECO:0005547 biological system reconstruction evidence based on inference from background scientific knowledge used in manual assertion](https://www.ebi.ac.uk/ols/ontologies/eco/terms?iri=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FECO_0005547).

### Species

**Multicellular organisms**

We curate to species level (e.g. *[Homo sapiens](https://www.uniprot.org/taxonomy/9606)*, *[Mus musculus](https://www.uniprot.org/taxonomy/10090)*, *[Caenorhabditis elegans](https://www.uniprot.org/taxonomy/6239)*).  

**Micro-organisms**

We curate to the model organism strain (e.g. [*Saccharomyces cerevisiae* (strain ATCC 204508 / S288c)](https://www.uniprot.org/taxonomy/559292), [*Escherichia coli* (strain K12)](https://www.uniprot.org/taxonomy/83333)).

In cases where a strain is not a model organisms but is of specific scientific interest we curate the complexes in the  species taxon and in the strain where the experimental evidence exists for the strain (e.g. [Human SARS coronavirus (SARS-CoV) species](https://www.uniprot.org/taxonomy/694009) and [SARS-CoV-2 strain](https://www.uniprot.org/taxonomy/2697049)).

##### Host-pathogen complexes

At the moment, each complex can only be assigned one species. In order to be able to combine all complexes for a given pathogen the complex is assigned the pathogen species.

### Complex Nomenclature

##### Complex recommended name

The most informative, well accepted name in the literature, that is intuitive to the user. Where possible, this will be the same as the equivalent component term in the [Gene Ontology](http://geneontology.org/). The term should always end in the word 'complex' or homo'n'mer. The recommended name is kept consistent when a complex is conserved across a taxonomic range. 

##### Complex systematic name

This is a string of gene symbols of the complex participants separated by a colon (e.g. "fiba:fibb:fibg") in alphanumeric order. The order is irrestective of species in a host-pathogen complex. Recommended gene symbols for each model organism will be used; therefore the systematic name may not be consistent when a complex is conserved across a taxonomic range. 

##### Complex synonym

All other possible names the complex is known by or can be described as.

##### Shortlabel (not displayed on website, only in download files)

An obligate part of the data model. An appropriate designation for the complex with species indicated using the UniProt five letter code e.g. fibrinogen_human, tfiid_mouse. When the same complex is conserved across a taxonomic range, the root name is maintained across all entries e.g. fibrinogen_human, fibrinogen_mouse, fibrinogen_bovin. 

The Shortlabel appears as "gene product name" when a Complex Portal AC is used as annotation object in Gene Ontology annotations.

### Complex Participants

##### Proteins

All proteins are derived from, and linked to, [UniProtKB](uniprot.org/) identifiers, ideally UniProtKB/Swiss-Prot. Isoform and chain designators are used when appropriate. Should one or more isoforms exist, annotation will be to the canonical protein entry unless either only one isoform is known to exist in the complex or different isoforms give the complex different properties. In the latter case, a separate entry should be made for each variation with detail given in the "Description" or "Properties" section as appropriate (see below for details on complex variants). 

##### Small molecules / polysaccharides

All small molecules are derived from, and linked to, [ChEBI](https://www.ebi.ac.uk/chebi/) identifiers. Small molecules are included only if they are integral to the complex or bind to the complex as part of its function, e.g. cofactors, electron donors/acceptors, such as ATP, H+. Enzyme targets are not added as participants. For example, ATP is entered as a cofactor if the enzyme function is NOT primarily an ATPase (e.g. [GyrA-GyrB DNA Gyrase complex](https://www.ebi.ac.uk/complexportal/complex/CPX-2177)) but NOT entered for ATPases where it is a substrate (e.g. [TRCF-UvrA complex](https://www.ebi.ac.uk/complexportal/complex/CPX-2155)). In the latter case the substrate is added using a [Gene Ontology](http://geneontology.org/) annotation, e.g. [ATP binding](https://www.ebi.ac.uk/QuickGO/term/GO:0005524).

##### Nucleic acids

Nucleic acids are only entered as participants when they are an obligate part of the complex. Non-coding RNA participants are linked to [RNACentral](https://rnacentral.org/) identifiers, all other nucleic acid types are created as generic molecules linked to generic [ChEBI](https://www.ebi.ac.uk/chebi/) identifiers. For complexes which assemble and then bind to a nucleic acids, this function is indicated in free text and annotated using [Gene Ontology](http://geneontology.org/) terms such as [DNA binding](https://www.ebi.ac.uk/QuickGO/term/GO:0003677).

###### Complex

A complex can also be a participant of a complex, e.g. [CMG-Pol epsilon complex](https://www.ebi.ac.uk/complexportal/complex/CPX-1556).

### Participant Features

- Any feature is mapped to the underlying sequence, as given in the source database, and cross-referenced to InterPro when possible. 
- If a PTM is required for complex formation or activation it is curated as a feature and the effects detailed in the "Properties" section.
- Binding regions or residues within proteins known to directly interact within the complex are shown as linked features in the graphical views.
- Stoichiometry is added when known. Stoichiometry=0 (or empty field on the website and single participant in the Complex Viewer) is used for participants with no information about stoichiometry. It is common that stoichiometry is only know for some participants in the same complex.

### Interaction Type

This is always 'Physical association', indicating that these proteins are present in the same complex.

### Free text annotation

##### Description

A brief, free-text description of the function of the complex, written in the same style as a UniProtKB/Swiss-Prot entry. For example "Required for processive DNA replication and may act as a replicative helicase during DNA synthesis. Plays a central role in S-phase genome stability.". 

##### Properties

Details of physical properties of the complex. This may include details about the topology, varying (as opposed to absolute) stoichiometry, molecular weight and Stoke's radius of the complex. 

##### Complex-assembly

Experimentally verified structural assembly e.g. homodimer, heterohexamer. Assemblies which have been computationally predicted are not included. 

##### Disease

Only added when the disease state has been specifically linked to the protein when in the complex. 

##### Ligand

Oe or more ligands transiently associated with this complex. They are usually linked to a [ChEBI](https://www.ebi.ac.uk/chebi/) identifier.

### Structured Annotations

All structured annotations are entered as database/controlled vocabulary cross-reference with an appropriate qualifier term.

##### Gene Ontology

Annotation to [Gene Ontology](http://geneontology.org) terms indicates the function, process, location and component of the complex as a whole. The Function term, in particular, may not be true for all members of the complex, for example enzyme complexes will be annotated with a catalytic function term even when some subunits play only a regulatory role. 

##### Experimental evidence

When high quality evidence for the existence of this complex is present in an [IMEx database](http://www.imexconsortium.org/), this will be added manually as a cross-reference so that it may be downloaded in the same file as the complex. 

##### 3D structures (crystals and EM structures)

Representative [wwPDB](https://www.ebi.ac.uk/pdbe/) and [EMDB](https://www.ebi.ac.uk/pdbe/emdb/) cross-references are added. Structures may represent the whole complex (qualifier = identity) or a partial complex (qualifier = subset). 

##### Evidence codes

The following [Evidence and Conclusion Ontology (ECO)](http://www.evidenceontology.org/) codes are used to indicate the strength of evidence that a complex exists: 

|ECO Code|Name|Description|
|--------|----|-----------|
|ECO:0000353|physical interaction evidence used in manual assertion|Used when experimental evidence for the complexes exists in a single experiment. The complex must be cross-referenced to experimental data in either an IMEx database, wwPDB or EMDB.|
|ECO:0005543|biological system reconstruction evidence by experimental evidence from mixed species used in manual assertion|Used when experimental evidence for the complexes exists in a single experiment but the constructs are derived from homologous gene products in different species. The complex must be cross-referenced to experimental in either an IMEx database, wwPDB or EMDB.|
|ECO:0005610|biological system reconstruction evidence based on homology evidence used in manual assertion|Used when experimental evidence exists for a complex in one species and it is desirable to curate a similar complex in another species for which only limited experimental evidence exists. Sequences and number of genome-encoded components are fairly conserved but some divergence may be observed. The complex with the experimental evidence must be annotated with ECO:0000353 or ECO:0005543 and has to be cross-referenced with the qualifier = "inferred-from".|
|ECO:0005544|biological system reconstruction evidence based on orthology evidence used in manual assertion|Used when experimental evidence exists for a complex in one species (e.g. human) and it is desirable to curate the same complex in another species for which only limited experimental evidence exists (e.g. mouse). Sequences are fairly conserved but some divergence may be observed and the number of genome-encoded components is identical. The complex with the experimental evidence must be annotated with ECO:0000353 or ECO:0005543 and has to be cross-referenced with the qualifier = "inferred-from".|
|ECO:0005546|biological system reconstruction evidence based on paralogy evidence used in manual assertion|Used when experimental evidence exists for a complex and it is desirable to curate a similar complex in the same species for which only limited experimental evidence exists. Sequences and number of genome-encoded components are fairly conserved but some divergence may be observed. The complex with the experimental evidence must be annotated with ECO:0000353 or ECO:0005543 and has to be cross-referenced with the qualifier = "inferred-from".|
|ECO:0005547|biological system reconstruction evidence based on inference from background scientific knowledge used in manual assertion|Used when no or only partial experimental evidence exists but the complex is generally assumed to exist. Functional studies or ligand binding evidence from pharmacological experiments are often used for the reconstruction of such complexes.|

##### Enzymatic activity

Catalytical complexes are annotated with appropriate E.C. numbers linked to [IntEnz](https://www.ebi.ac.uk/intenz/) and reactions in [Rhea](https://www.rhea-db.org/).

##### Additional literature

Articles covering further experimental or functional information and review articles are added and lonked to [EuropePMC](http://europepmc.org/). 

##### Pathway information

For human complexes, crosslinks to [Reactome](https://reactome.org/) put complexes into a pathway context. Note that the definition of a complex is different in Reactome and in many cases a one-to-many relationship exists. 

##### Disease information

Cross references to the [Experimental Factor Ontology (EFO)](https://www.ebi.ac.uk/efo/) or their contributing databases (e.g. Orphanet, Human Phenotype Ontology) are added if a complex has been linked to a specific disease condition. 

##### Drug target information

Cross-links to [ChEMBL](https://www.ebi.ac.uk/chembl/) are used to indicate complexes which have been used as drug targets. 

### Complex Variants

If variant forms of a complex exist i.e. the same functional unit can exist in alternate forms with differing macromolecular composition, these are curated as separate objects. For example, PDGF can exist as a PDGF-A homodimer, PDGF-B homodimer, PDGF-AB heterodimer, PDGF-C homodimer and a PDGF-D homodimer. If the variants have well-accepted names, e.g. PDGF-AB, these may be used as the primary name. If not, then the recommended name is qualified by variant 1, variant 2 e.g. [TRAMP complex variant 1](https://www.ebi.ac.uk/complexportal/complex/CPX-1678).

### Versioning

A version is identified by a .x suffix (where x is a number) of the accession number. The version is included in the download files but not displayed on the website.

A complex receives a new version if its participants change (adding or removing one or more participants) or its function is redefined. 
