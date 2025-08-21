# Galaxy Cluster Outer Regions Research

A collaborative research project analyzing multi-wavelength observations (optical, X-ray, SZ) to understand the thermodynamic properties and gas distribution in the outskirts of galaxy clusters.

## Research Goals

1. Characterize the gas density and temperature profiles in cluster outskirts
2. Study the connection between the intracluster medium and large-scale structure
3. Investigate the impact of cluster dynamics on gas properties
4. Compare observations with theoretical predictions and simulations

## Project Structure

```
.
├── data/                     # Data storage (see data_management.md)
│   ├── raw/                  # Original, unmodified data
│   ├── processed/            # Processed data products
│   └── external/             # External datasets or references
├── docs/                     # Documentation
│   ├── meetings/             # Meeting notes and minutes
│   ├── papers/               # Relevant literature
│   ├── proposals/            # Observation proposals
│   └── data_management.md    # Data organization and handling
├── notebooks/                # Jupyter notebooks for analysis
│   ├── 01_data_exploration/  # Initial data inspection
│   ├── 02_analysis/         # Data analysis workflows
│   └── 03_visualization/     # Figures and plots
├── scripts/                  # Reusable analysis scripts
├── environment.yml           # Conda environment specification
└── README.md                 # This file
```

## Getting Started

1. Clone this repository
2. Set up the conda environment: `conda env create -f environment.yml`
3. Activate the environment: `conda activate cluster-outer-profile`
4. Start Jupyter Lab: `jupyter lab`

## Data Management

See `docs/data_management.md` for guidelines on:
- Data organization and naming conventions
- Data processing workflows
- Version control for large datasets
- Data sharing and backup procedures

## Contributing

Please read `CONTRIBUTING.md` for our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.
