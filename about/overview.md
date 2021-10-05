## Overview of Complex Portal

The Complex Portal is a manually curated, encyclopaedic resource of macromolecular complexes from a number of key model organisms. 

Complexes are defined as an assembly of any two or more proteins and/or nucleic acids that are stable enough in vitro to be reconstituted and have been demonstrated to have a specific molecular function. They may also contain small molecules if they are essential, functional components.

All complexes are derived from physical molecular interaction evidences extracted and cross-referenced from the literature and cross-referenced to the Molecular Interaction Database [IntAct](https://www.ebi.ac.uk/intact/) where available, or by curator inference from information on homologs in closely related species or by inference from scientific background. All complexes are tagged with [Evidence and Conclusion Ontology](https://www.ebi.ac.uk/ols/ontologies/eco) codes to indicate the type of evidence available for each entry.

**Special considerations:**

- Stoichiometry is only included when it has been directly determined experimentally.

- Kinetic data is not included but can be found in [IntAct](https://www.ebi.ac.uk/intact/) if a related publication has been curated there. 

- Transient complexes such as enzyme-substrate assemblies or pre-assembly structures of large machineries are not curated. 

- Large, multi-complex machineries are reduced to their functional subcomplexes both for ease of annotation and also because the final assemblies are often dynamic, rather than a single instance of a functional unit existing at any moment of time. The subcomplexes of large assemblies are annotated with GO terms relating to the larger machineries, for example, all [spliceosome sub-complexes](https://www.ebi.ac.uk/complexportal/complex/search?query=GO:0005681&page=1) are annotated with the GO term [GO:0005681 spliceosomal complex](https://www.ebi.ac.uk/QuickGO/term/GO:0005681) to facilitate searching.

- Homomultimers are only curated if it has been demonstrated experimentally that multimerization is required for its function or when there was a heterodimeric complex and at least one of the two participants formed an orthologous homodimeric complex. This strategy was adopted because it is often difficult to prove experimentally that a protein must form a homomer to be functionally active, because some homomers don’t become active until they are part of a bigger assembly. 

- Homomultimeric polymers and filaments are not curated.

- Judgment of what constitutes a stable complex is based on a consensus decision made by two curators.

More information on our curation rules can be found [here](https://www.ebi.ac.uk/complexportal/documentation#data_content).
