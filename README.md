## iUmbe1-GEM: Genome-scale metabolic model of *Umbelopsis* sp. WA50703 
<!--
[![Version](https://badge.fury.io/gh/{{organization or username}}%2F{{repository name}}.svg)](https://badge.fury.io/gh/sysbiochalmers/yeast-gem)  
[![Zenodo](https://zenodo.org/badge/{{Zenodo ID}}.svg)](https://zenodo.org/badge/latestdoi/{{Zenodo ID}}) 
-->

#### Description

Oleaginous fungi, known for their high lipid content—up to 80% of their dry mass—are of significant interest for biotechnological applications, particularly in biofuel and fatty acid production. Among these, the genus Umbelopsis, a common soil saprotroph of the Mucoromycota phylum, stands out for its rapid growth, low nutritional requirements, and ability to produce substantial amounts of lipids, especially polyunsaturated fatty acids (PUFAs). Despite previous studies on lipid production in Umbelopsis, metabolic engineering has been underexplored. This study fills that gap by presenting the first comprehensive metabolic model for Umbelopsis sp. WA50703, encompassing 2413 metabolites, 2216 reactions, and 1629 genes (iUmbe1). The model demonstrated strong predictive accuracy, correctly predicting metabolic capabilities in 82.1% of cases when evaluated against experimental data. Using the Flux Scanning based on Enforced Objective Flux (FSEOF) algorithm, the study identified 33 genes linked to 23 metabolic reactions. Notably, reactions catalysed by acetyl-CoA carboxylase and carbonic anhydrase emerged as prime candidates for up-regulation. These findings provide a solid framework for future metabolic engineering efforts to optimize PUFA production in Umbelopsis strains.

To improve usability, we have developed a streamlined version of the model (iUmbe1-slim) that excludes reactions linked to orphan metabolites. This refined version facilitates optimization analyses and has been made available in the repository for reference and further use. At the same time, the repository contains the full version of the model (iUmbe1), which includes all orphan metabolites and their associated reactions. The full version is essential for future model expansions, ensuring a complete representation of the metabolic network.
The full model contains all reactions that are supported by at least one gene, as they are backed by genomic evidence and indicate potential biological relevance. Keeping these reactions ensures the model remains adaptable, allowing for future discoveries that may establish new connections between currently orphaned metabolites and broader metabolic pathways.
 

#### Citation

  > Dziurzyński, M., Nowak, M. E., Furman, M., Okrasińska, A., Pawłowska, J., & Fondi, M. Insights into optimization of oleaginous fungi – genome-scale metabolic reconstruction and analysis of *Umbelopsis* sp. WA50703. bioRxiv.  [doi:https://doi.org/10.1101/2024.10.01.616082](https://www.biorxiv.org/content/10.1101/2024.10.01.616082v1.full)



#### Keywords

Metabolic modeling; Lipid synthesis; Biotechnology; Filamentous fungi; Fatty acids

**Utilisation:** experimental data reconstruction; multi-omics integrative analysis; _in silico_ strain design; model template   
**Field:** metabolic-network reconstruction   
**Type of model:** reconstruction; curated  
**Omic source:** genomics; transcriptomics, phenomics  
**Taxonomic name:** _Umbelopsis_  sp. WA50703  
**Taxonomy ID:** [taxonomy:3097288](https://identifiers.org/taxonomy:3097288)  
**Genome ID:** [insdc.gca:GCA_964291815.1](https://identifiers.org/insdc.gca:GCA_964291815.1)  
**Metabolic system:** general metabolism  
**Strain:** WA50703  
**Condition:** aerobic; minimal synthetic medium  


### Installation

The model can be read and analysed using [COBRApy](https://github.com/opencobra/cobrapy), a community-driven Python package for constraint-based modeling of metabolic networks.


### Usage

```
import cobra
from cobra.io import read_sbml_model
model = read_sbml_model("iUmbe1.smbl")
model.optimize()
```

### Contributing

Contributions are always welcome! Please read the [contributing guideline](.github/CONTRIBUTING.md) to get started.


### Contributors

[Contributors](https://github.com/mdziurzynski/iUmbe1-GEM/graphs/contributors)