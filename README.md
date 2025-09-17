# Galaxy Cluster Outer Regions Research

A collaborative research project analyzing multi-wavelength observations (optical, X-ray, SZ) to understand the gas properties and distribution in the outskirts of galaxy clusters.

## Research Goals

1. Characterize the gas density and temperature profiles at cluster outskirts

### tasks:

- [x] catalogues matching and selection
- [ ] understanding and setting the centres
- [ ] understanding and setting the scale radii 
- [ ] outside object removing/fitting 2 halo term 
- [ ] background subtraction and masking
- [ ] stacking images for profiles 
- [ ] comparisons with simulation results


## Project Structure

```
.
├── data/                     # Data storage (see data_management.md)
│   ├── DESI/                  # DESI galaxy cluster catalogues
│   ├── ACT/                   # ACT catalogues
│   └── eROSITA/               # eROSITA catalogues
├── scripts/                # Jupyter notebooks for analysis
│   ├── 01_data_exploration/  # Initial data inspection
│   ├── 02_analysis/         # Data analysis workflows
│   └── 03_visualization/     # Figures and plots
└── README.md                 # This file
```

## Data Management

See `README.md` in data/ for guidelines on:
- Data organization and naming conventions
- Data processing workflows
- Version control for large datasets
- Data sharing and backup procedures

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.
