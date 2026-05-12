# GlmUpred: A Web Server for Predicting Inhibitors Against Bacterial Target GlmU

Welcome to the official documentation for **GlmUpred**, a specialized computational resource developed to identify and design inhibitors against the bacterial GlmU protein. The GlmU protein is a bifunctional enzyme essential for the synthesis of peptidoglycan and lipopolysaccharide in bacteria, making it an attractive target for developing new antibacterial agents, particularly against drug-resistant strains like *Mycobacterium tuberculosis*.

**Web Server:** [http://crdd.osdd.net/raghava/glmupred/](http://crdd.osdd.net/raghava/glmupred/)

---

## Citation

Singla, D., Anurag, M., Dash, D., & Raghava, G. P. S. (2011). 
**A web server for predicting inhibitors against bacterial target GlmU protein.** *BMC Pharmacology*, 11, 5. 
[https://doi.org/10.1186/1471-2210-11-5](https://doi.org/10.1186/1471-2210-11-5)

---

## About the Platform

The emergence of drug-resistant bacteria poses a global health threat. GlmUpred addresses this by providing a platform to predict the inhibitory activity ($IC_{50}$) of chemical compounds against the GlmU protein. The platform utilizes both Quantitative Structure-Activity Relationship (QSAR) and molecular docking techniques to provide a multi-faceted evaluation of potential inhibitors.

### Key Features
* **QSAR Modeling**: Predicts inhibitory activity based on molecular descriptors calculated from the chemical structure.
* **Docking Integration**: Incorporates docking energies into the prediction models to account for the structural fit within the GlmU active site.
* **Diverse Training Data**: Models were trained on 84 diverse GlmU inhibitors retrieved from PubChem BioAssay.

---

## Technical Overview

The performance of GlmUpred is based on sophisticated machine learning models that link chemical features to biological activity.

| Model Type | Descriptors | Correlation ($r$) |
| :--- | :--- | :--- |
| **Docking-based** | AutoDock Energies | 0.35 |
| **Descriptor-based** | CDK & PaDEL Descriptors | 0.81 |
| **Hybrid** | Mixed Descriptors | 0.81 |

---

## Model Functionality

* **Activity Prediction**: Users can submit the structure of a chemical compound (in SMILES or SDF format) to predict its potential $pIC_{50}$ against GlmU.
* **Molecular Descriptors**: The server calculates a wide range of descriptors including constitutional, topological, and geometric properties.
* **Target Specificity**: Specifically optimized for the C-terminal uridylyltransferase domain of the GlmU protein.

---

## Applications

* **Antibiotic Discovery**: Screening large chemical libraries to find novel leads against tuberculosis and other bacterial infections.
* **Lead Optimization**: Assisting medicinal chemists in modifying compounds to increase their potency against the GlmU target.
* **Computational Biology**: Providing a specialized tool for studying the structure-activity relationships of bacterial enzyme inhibitors.

---

## Contact & Authors

**Prof. Gajendra P. S. Raghava**
Bioinformatics Centre, Institute of Microbial Technology, Sector 39A, Chandigarh, India.
**Email**: raghava@imtech.res.in

---

## License

This resource is open-access and distributed under the terms of the **Creative Commons Attribution License**, permitting unrestricted use and distribution provided the original work is properly credited.
