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

LEAD-EA/
│── dataset/                # Benchmark instances (TA01–TA20)
│── algorithmlib.py         # Core algorithmic components
│── cp_model.py             # CP model implementation
│── milp_model.py           # MILP model implementation
│── main.py                 # Main entry for running LEAD-EA

---

## Requirements
numpy==1.24.3
shap==0.49.1
openai==2.29.0
scikit-learn==1.7.2
docplex==2.31.254

---

## How to run results
Run the MILP model
python milp_model.py
Run the CP model
python cp_model.py
Run LEAD-EA
python main.py

---

## Dataset
Benchmark instances are provided in the dataset/ directory.
Please ensure the dataset path is correctly specified before running experiments.


## Important Note on Code Availability
The current repository provides the implementation of the MILP model, CP model, and the LEAD-EA framework.
However, the context-aware code correction module used in LEAD-EA is not included in this release.
This component relies on a dataset of code correction examples constructed through data collection and preprocessing. 
Due to the substantial effort required to build and maintain this dataset, it is not included in the current release.

## Related Work
This repository is associated with ongoing research on JSP-SDST and automated algorithm design.
The corresponding manuscript is currently under review and will be made publicly available upon acceptance.

## Citation
If you find this repository useful, please consider citing:

@article{yourpaper2026,
  title={Your Paper Title},
  author={Author1 and Author2 and Author3},
  journal={Under Review},
  year={2026}
}

## Contact
For questions or collaborations, please contact:
Weiyao Cheng: weiyao_cheng@163.com
