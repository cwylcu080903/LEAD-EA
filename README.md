# LEAD-EA

This repository provides the implementation of the MILP model, CP model, and LEAD-EA for solving the job shop scheduling problem with sequence-dependent setup times (JSP-SDST).

---

## Overview

This project includes three main components:

- **MILP model**: a mixed-integer linear programming model for JSP-SDST  
- **CP model**: a constraint programming model for JSP-SDST  
- **LEAD-EA**: a large language model (LLM)-driven automated evolutionary algorithm design framework  

LEAD-EA is designed to automatically generate and refine evolutionary algorithms by jointly evolving algorithm configurations and structures.

---

## Repository Structure

```text
EvoPlace/
│── dataset/                # Benchmark instances (TA01–TA20)
│── algorithmlib.py         # Core algorithmic components
│── cp_model.py             # CP model implementation
│── milp_model.py           # MILP model implementation
│── main.py                 # Main entry for running LEAD-EA
Requirements

Install Python dependencies:

pip install -r requirements.txt
Additional requirements

The MILP and CP models rely on IBM ILOG CPLEX Optimization Studio, including:

CPLEX Optimizer
CP Optimizer

Please ensure they are properly installed and configured.

Usage
Run the MILP model
python milp_model.py
Run the CP model
python cp_model.py
Run LEAD-EA
python main.py
Dataset

Benchmark instances are provided in the dataset/ directory.

Please ensure the dataset path is correctly specified before running experiments.

Reproducibility

To reproduce the experimental results:

Install all required dependencies
Prepare the dataset in the dataset/ folder
Run the corresponding scripts for MILP, CP, or LEAD-EA

Due to stochastic components in LEAD-EA, multiple runs may be required to obtain stable results.

Important Note on Code Availability

The current repository provides the full implementation of the MILP model, CP model, and the LEAD-EA framework.

However, the context-aware code correction module used in LEAD-EA is not included in this release.
This component relies on a curated dataset of code correction examples constructed from extensive data collection and preprocessing.

We are actively working on this direction and plan to release a more complete version in future work.

Related Work

This repository is associated with ongoing research on JSP-SDST and automated algorithm design.

The corresponding manuscript is currently under review and will be made publicly available upon acceptance.

Citation

If you find this repository useful, please consider citing:

@article{yourpaper2026,
  title={Your Paper Title},
  author={Author1 and Author2 and Author3},
  journal={Under Review},
  year={2026}
}
Contact

For questions or collaborations, please contact:

Your Name: your_email@example.com
License

This project is released under the MIT License.
