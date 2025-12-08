# Pathway-centered abstraction of BioPAX models

This repository contains codes to generate a pathway-centered abstraction of Reactome BioPAX data.

Download the Reactome BioPAX export in a folder named `BioPAXData/`.

- The script `01_generate_pathway_abstraction.ipynb` allows to generate a pathway-centered abstraction with two types of relations: 
    - The relation `abstraction:IsAChildOf` describes the hierarchical relationships between pathways
    - The relation `abstraction:NextStepPathway` describes the sequential relationships between pathways

The pathway-centered abstraction file is generated in the `Results/ReactomeHomoSapiens94Abstractions` folder.

- The script `02_weight_pathway_abstraction.ipynb` allows to weight the `abstraction:NextStepPathway` relationships in the pathway abstraction for them to reflect the biological distance of pathways. Several metrics are tested in the script. 

The weighted pathway-abstraction files are generated in the `Results/ReactomeHomoSapiensWeightedAbstractions` folder.