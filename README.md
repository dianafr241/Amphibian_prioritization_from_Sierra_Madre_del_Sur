# Amphibian prioritization from Sierra Madre del Sur, Mexico 
---

These data are part of the master's project entitled: “Priorizacion espacial para la conservación de anfibios en la Sierra Madre del Sur con escenarios futuros de cambios globales”. This project was developed within the Master's Program in Biological Sciences of the National Autonomous University of Mexico by Diana L. Fuentes-de la Rosa, et al. The project aims i) to evaluate the performance of the current protected area network and ii) to identify potential areas for expansion of the current protected network contemplating their persistence in time.
For this, species distribution models and buffers were made for the amphibians of the SMS. Moreover, current and future (2060) land use layers were incorporated. Each layer was weighed, and four spatial prioritizations were run in the Zonation 4.0.0 program. Two contemplate the entire area of the SMS (unconstrained settings), while the remaining two (constrained settings) exclude the polygons of the current Protected Areas and Areas Voluntarily Destined for Conservation according to the National Commission of Natural Protected Areas (CONANP, 2022).

>## Description of the Data and file structure

The files are divided into two kinds: files with the parameters inputs of each analysis and the others containing features layers such as land use layers (2060) and species distribution models (.asc). Note that ABF refers to Additive Benefit Function and CAZ refers to Core Area Zonation; both are cell removal rule algorithms of Zonation software.

Species distribution models were fitted using single occurrence data from 44 scientific collections. For each species, the distribution was reviewed with literature. In addition, historical accessibility was considered, restricting the projection to the hydrological basins. We used the CHELSA variables and selected those that did not covary with each other. We use the MaxEnt algorithm to perform the correlative models.

On the other hand, round buffers of 2.5 km in diameter were made for species with less than ten records as a conservative estimate of their distribution ranges.

Baseline land use was taken from the National Institute of Statistics and Geography (INEGI 2016), and land use change predictions were provided directly by Mendoza-Ponce et al., 2018.
The protected area mask (ANP_ADVC.asc) was made by joining the polygons of all protected areas registered by CONANP that intersect with the Sierra Madre del Sur polygon.
The .dat files are the configuration of each analysis.
The .spp file are a list of the features used for each analysis. In this case, they are composed of 107 amphibian species, a layer of current land use, and three models of change in land use by 2060 (Green, Busissnes As Usual and Worst).
The .bat files are command lines for each analysis.
The .txt file grouping the features of each analysis by taxonomic family, except for the land use layers.

These data can be analyzed with the Zonation 4.0.0 software.


>#### Abbreviations:

 - C: Constrained run
 - U: Unconstrained run
 - ABF: Additive Benefit Function
 - CAZ refers to Core Area Zonation
 - BAU: Busissnes As Usual
 - SMS: Sierra Madre del Sur

>#### References

CONANP, 2022. Áreas Naturales Protegidas. Información espacial de las Áreas Naturales
Protegidas [WWW Document]. URL
http://sig.conanp.gob.mx/website/pagsig/info_shape.htm (accessed 10.14.22).

INEGI, 2016. Conjunto de Datos Vectoriales de Uso del Suelo y Vegetación. Instituto.pdf.

Mendoza-Ponce, A., Corona-Núñez, R., Kraxner, F., Leduc, S., Patrizio, P., 2018. Identifying
effects of land use cover changes and climate change on terrestrial ecosystems and carbon
stocks in Mexico. Glob. Environ. Change 53, 12–23.
https://doi.org/10.1016/j.gloenvcha.2018.08.004



