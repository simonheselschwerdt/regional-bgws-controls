# regional-bgws-controls

Code accompanying the manuscript:

**Regional controls on blue-green water partitioning under climate change**

Simon P. Heselschwerdt, Abhinav Dengri, Chiara M. Holgate, and Peter Greve

---

## Description

This repository contains the code used to analyse projected changes in blue–green water partitioning under climate change and to generate the figures presented in the manuscript:

> Heselschwerdt, S. P., Dengri, A., Holgate, C. M., and Greve, P.
> Regional controls on blue-green water partitioning under climate change.
> Submitted to Geophysical Research Letters (2026).

The analysis is based on CMIP6 Earth System Model simulations and focuses on regional changes in the partitioning of precipitation between runoff (blue water) and transpiration (green water).

This repository is intended to support transparency and reproducibility of the published results.

---

## Repository status

This repository is currently under development and will be updated following manuscript review.

The current version contains the core analysis scripts and environment specification required to reproduce the main results.

---

## Data availability

The original CMIP6 model output used in this study is not distributed through this repository.

CMIP6 data can be accessed through the Earth System Grid Federation (ESGF) and the DKRZ CMIP Data Pool.

Additional data sources used in the manuscript are described in the manuscript's Data Availability Statement.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/simonheselschwerdt/regional-bgws-controls.git
cd regional-bgws-controls
```

Create the conda environment:

```bash
conda env create -f environment.yml
conda activate regional-bgws-controls
```

---

## Usage

The analysis workflow is primarily notebook-based.

After configuring local data paths, notebooks can be executed to:

- preprocess model data
- calculate blue–green water partitioning metrics
- perform regional analyses
- generate manuscript figures

---

## Directory structure

```text
regional-bgws-controls/
├── notebooks/
├── src/
├── environment.yml
├── LICENSE
└── README.md
```

---

## Authors

Simon P. Heselschwerdt (corresponding author)

Climate Service Center Germany (GERICS)
Helmholtz-Zentrum Hereon

Contact:
simon.heselschwerdt@hereon.de

---

## License

This project is licensed under the MIT License.
