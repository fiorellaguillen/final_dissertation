# Final_dissertation


## Setup and Requirements

This repository relies on a specific Python environment and a set of pre-downloaded data files. Please follow these steps before running the notebooks:

### Environment

Create a new conda environment using the provided environment.yml file.

conda env create -f environment.yml
conda activate porosity-env


This ensures compatibility with all required libraries (PyTorch, segmentation models, GIS libraries, etc.).

### Data

All data required to run the notebooks has been uploaded to this OneDrive folder
[OneDrive link](https://1drv.ms/f/c/4c6a6da74e365895/Eqz4AqdmEwBGmbCQacSWJU0BoM4fBznq1S6KsvJ29zpQfw?e=mvMM8a)

Please download the entire directory and place it under the same folder structure as referenced in the notebooks.´

```text
dissertation_rfgh/
│
├── base_data/                          # Base datasets provided for reproducibility
├── best_deeplabmodels/                 # Trained DeepLabV3+ model versions
├── inference/                          # Breña's inference outputs on panoramas
├── panos/                              # Breña's raw Mapillary panoramas
├── python_notebooks/                   # Jupyter notebooks for each stage - Also available on Github (https://github.com/fiorellaguillen/final_dissertation)
├── test_results/                       # Evaluation results of trained models
├── training_images/                    # Training dataset images
├── training_stats/                     # Logs and statistics from training runs
└── environment.yml                     # Conda environment specification

This guarantees reproducibility and avoids inconsistencies from querying external APIs (e.g., Mapillary).

### Notebook execution

Notebooks labeled with (SKIP) at the beginning of a section indicate that the code can be skipped, as the required processed files are already included in the shared folder. They have been already commented out.

You may still run them if you wish to replicate the data collection process, but doing so requires valid API tokens and may yield slightly different results due to updated external data.
