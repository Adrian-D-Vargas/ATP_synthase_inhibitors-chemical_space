# Chemioinformatics Workflow

This repository contains all code, data, and analysis workflows used in the scientific article:

**"Exploring the chemical space of ATP synthase inhibitors: a chemoinformatics approach"**

## Overview
This project provides a complete cheminformatics pipeline for the curation, descriptor calculation, scaffold analysis, and visualization of ATP synthase inhibitors and DrugBank compounds. The workflow is implemented in Python using Jupyter Notebooks and leverages RDKit, pandas, matplotlib, seaborn, and scikit-learn.

## Main Features
- **Dataset curation:** Removal of duplicates, salts, and inorganic/organometallic compounds; addition of explicit hydrogens.
- **Descriptor calculation:** Lipinski, TPSA, logP, rotatable bonds, H-bond donors/acceptors.
- **Scaffold analysis:** Bemis-Murcko scaffold extraction and frequency analysis.
- **Activity landscape:** Activity cliff detection and visualization.
- **Chemical space visualization:** PCA and t-SNE plots for both ATP synthase inhibitors and DrugBank compounds.
- **Exported results:** All key results are saved as CSV files for reproducibility and further analysis.

## Structure
- `workflow.ipynb`: Main Jupyter Notebook containing all code and analysis steps.
- `DataBase/`: Folder containing curated datasets and raw input files.
- `*.csv`: Output files with curated data, descriptors, scaffold frequencies, and activity cliffs.

## Data Availability
- **DrugBank dataset:** Due to licensing restrictions, we cannot share the DrugBank dataset in this repository. If you wish to use DrugBank data, you must request access directly from [DrugBank](https://go.drugbank.com/releases/latest).
- **ATP synthase inhibitors dataset:** Provided in the repository for full reproducibility.

## Requirements
All required libraries and their exact versions are specified in `requirements.txt`. Main packages include:
- Python 3.13.1
- RDKit 2024.09.6
- pandas 2.2.3
- matplotlib 3.10.0
- seaborn 0.13.2
- scikit-learn 1.6.1

For full reproducibility, please use the provided `requirements.txt` to create your environment with conda.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   ```
2. Create the environment using conda and the provided requirements file:
   ```bash
   conda create --name chemioinformatics-env --file requirements.txt
   ```
3. Activate the environment:
   ```bash
   conda activate chemioinformatics-env
   ```
4. Open `workflow.ipynb` in Jupyter and run all cells.

## Scientific Context
This repository supports the publication of a scientific article focused on the chemioinformatic characterization of ATP synthase inhibitors, including comparison with DrugBank compounds. All scripts and data are provided for full reproducibility.

## Authors
- Adrian Durán-Vargas
- Luis F. Cofas-Vargas
- Juan F. Avellaneda-Tamayo
- Jesús A. Rauda-Ceja
- Paola Mendoza-Espinosa
- José L. Medina-Franco
- Enrique García-Hernández

## License
This project is released under the MIT License.

## Contact
For questions or collaboration, please contact: adv291882@gmail.com
