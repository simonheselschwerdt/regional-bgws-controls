# **LUMIP_bgws** [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18378689.svg)](https://doi.org/10.5281/zenodo.18378689)

## **Preliminary Title**
**Global impacts of land-use and land-cover change on blue-green water partitioning**

---

## Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Usage of notebooks](#usage-of-notebooks)
- [Directory Structure](#directory-structure)
- [Authors and Acknowledgment](#authors-and-acknowledgment)
- [License](#license)

## Description
This repository contains code to reproduce the findings of the work in preliminary manuscript 'Global impacts of land-use and land-cover change on blue-green water partitioning' (by Simon P. Heselschwerdt*, Abhinav Dengri, Nora L. S. Fahrenbach, and Peter Greve), and this README describes the code and data for reproducibility.

### **Notebook-Centric Workflow**
The project uses Jupyter notebooks for all major tasks, including data ingestion, preprocessing, analysis, and visualization. The `src` directory stores reusable functions and utilities to support the notebooks, ensuring modular and clean code.

### **Code availability**
We provide all code to reproduce the main results and all figures of the paper. Either browse/download files individually or clone the repository to your local machine (see installation). 

### **Data availability** 
Due to storage and copyright constraints, original CMIP6 and LUH2 data have to be downloaded from their original sources (given in Data Availability Statement).

## Installation

Follow these steps to set up the project locally:

1. **Clone the repository:**
   ```plaintext
   git clone https://github.com/simonheselschwerdt/LUMIP_bgws.git
   cd bgws_analysis
   ```
2. **Set up a Conda environment:**
   ```plaintext
   conda env create -f environment.yml
   conda activate bgws_analysis
   ```
3. **Verify installation: Ensure all dependencies are installed by running:**
   ```plaintext
   python --version
   jupyter --version
   ```
## Usage of notebooks

1. **Download and Preprocess Data**
   - *Define your data directory in the configuration file (src/config.py) first.*
   - Use the following notebook to download and preprocess the required datasets:
     ```plaintext
     notebooks/import_and_preprocess.ipynb
     ```
2. **Generate Figures and Tables**
   - Create all figures of the publication:
     ```plaintext 
     notebooks/get_figures_and_tables.ipynb
     ```
## Directory Structure

```plaintext
bgws-analysis/
├── notebooks/                                      
│   │   ├── import_and_preprocess.ipynb    
│   │   └── get_figures_and_tables.ipynb
├── src/                                            
│   ├── __init__.py                               # Package initialization
│   ├── config.py                                 # Configuration file for defining directories and parameters
│   ├── data_handling/
│   │   ├── __init__.py
│   │   ├── import_data.py
│   │   ├── load_data.py
│   │   ├── compute_statistics.py        
│   │   ├── process_data.py
│   │   └── save_data_as_nc.py
│   ├── visualization/ 
│   │   ├── __init__.py
│   │   ├── global_maps_and_tabels.py
│   │   └── colormaps.py      
├── environment.yml                               # Conda environment specification
├── LICENSE                                       # License file
└── README.md                                     # Project documentation
```            

## Authors and acknowledgment
The Github repository is maintained by the corresponding author (Simon P. Heselschwerdt, Email: [simon.heselschwerdt@hereon.de](mailto:simon.heselschwerdt@hereon.de)). 
All acknowledgements and references will be available in the published paper.

## License
This project is licensed under the [MIT License](LICENSE).
