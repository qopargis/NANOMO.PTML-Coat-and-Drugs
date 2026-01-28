# NANOMO.PTML-Coat-and-Drugs
NANOMO.PTML Coat and Drugs model development

# Predicting Coated-Nanoparticle Drugs Release Systems with Perturbation-Theory Machine Learning (PTML) Models

# Authors: Ricardo Santana*a,b, Robin Zuluaga c, Piedad Gañán b, Sonia Arrasate d, Enrique Onieva a, and Humbert González-Díaz*,e,f

# Affiliations:
a University of Deusto, Avda. Universidades, 24, 48007 Bilbao, Spain.
b Grupo de Investigación Sobre Nuevos Materiales, Facultad de Ingeniería Química, Universidad Pontificia Bolivariana, Circular 1° N° 70-01, Medellín, Colombia.
c Facultad de Ingeniería Agroindustrial, Universidad Pontificia Bolivariana, Circular 1° N° 70-01, Medellín, Colombia.
d Department of Organic Chemistry II, University of the Basque Country UPV/EHU, 48940, Leioa, Spain.
e IKERBASQUE, Basque Foundation for Science, 48011, Bilbao, Spain.
f Biofisika Institue CSIC-UPVEHU, University of Basque Country UPV/EHU, 48940, Leioa, Spain.

# Paper Reference
	Nanoscale, 2020,12, 13471-13483. doi: https://doi.org/10.1039/D0NR01849J

# ABSTRACT.
Nanoparticles (NPs), decorated with coating agents (polymers, gels, proteins, etc.), form Nanoparticle Drug Delivery Systems (DDNS) of high interest in Nanotechnology and Biomaterials science. There is an increasing publication of experimental data sets of biological activity, toxicity, and delivery properties of DDNS. However, these data sets are still disperse and no as large as the datasets of DDNS components (NP and drugs). This prompts researchers train Machine Learning (ML) algorithms able to design new DDNS based on the properties of their components. However, most ML models reported up to date predict specific activities of NP or drugs over determined target or cell line. In this paper, we combine Perturbation Theory and Machine Learning (PTML algorithm) to train a model able to predicting the best components (NP, coating agent, and drug) for DDNS design. In so doing, we downloaded from ChEMBL a dataset of >30000 preclinical assays of drugs. We also downloaded from public sources a NPs data set formed by preclinical assays of coated Metal Oxide Nanoparticles (MONPs). Both, drugs and NPs datasets of preclinical assays cover multiple conditions of assay that can be listed as two arrays cjdrug and cjNP, respectively. The cjdrug array includes >504 biological activity parameters (c0drug), >340 target proteins (c1drug), >650 types of cells (c2drug), >120 assay organisms (c3drug), > 60 assay strains (c4drug). On the other side, the cjNP array includes 3 biological activity parameters (c0NP), 40 types of proteins (c1NP), 10 shapes of nanoparticles (c2NP), 6 assay media (c3NP), and 12 coating agents (c4NP). After downloading, we pre-processed both data sets by separate calculating PT operators able to account for changes (perturbations) in drug, coating agents, and NP chemical structure and/or physicochemical properties as well as for assay conditions. Next, we carry out an information fusion process forming a final dataset of above 500000 DDNS (drug + MONP pairs). We also trained other linear and non-linear PTML models using R studio scripts for comparative purposes. Until the best of our knowledge, this is the first multi-label PTML model useful to select drugs, coating agents, and metal or metal-oxide nanoparticles to be assembled in order to design new DDNS with optimal activity/toxicity profiles.

# Supporting Information
The dataset used, including molecular descriptors, and assay conditions, desirability, cutoff, biological activities etc., was included in tables Table S1, Table S2 and Table S3 (SI01.xlsx). See details about these Moving Average operators on Table 3 and Table 5 (see Table S1 and Table S2 respectively in supporting information for full dataset consultation). In addition, Table S3 we also included all details about each case, observed classification, predicted classification, input variables, experimental conditions, drug derivative and nanoparticle characteristics. This table is freely available online in the public data repository Figshare with doi: https://doi.org/10.6084/m9.figshare.8143394.v1, due to volume restrictions. Paper supporting info is available open access as well. https://pubs.rsc.org/en/content/articlelanding/2020/nr/d0nr01849j/

# ■ AUTHORS INFORMATION
Corresponding author
*(H.G.D) E-mail: humberto.gonzalezdiaz@ehu.es (H.G.-D.)
  Orcid: 0000-0002-9392-2797
*(R.S) E-mail: ricardo.santana@opendeusto.es (R.S.)
  Orcid: 0000-0002-5206-2305
  
# ■ ACKNOWLEDGMENTS
R.S.C. thanks COLCIENCIAS scholarship for the doctorate studies; “Convocatoria para Doctorado Nacional 757” from 2017. This original research is part of the project “Investigación en Derecho Internacional y Nanotecnología” registered in the Research Centre of Universidad Pontificia Bolivariana with register number 766B-06/17-37. Special gratitude is extended to CYTED NANOCELIA network. The authors acknowledge research grants from Ministry of Economy and Competitiveness, MINECO, Spain (FEDER CTQ2016-74881-P) and Basque government (IT1045-16). The authors also acknowledge the support of Ikerbasque, Basque Foundation for Science. The authors also acknowledge the support of Ikerbasque, Basque Foundation for Science.
