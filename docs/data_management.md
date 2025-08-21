# Data Management Plan

This document outlines the procedures for handling data in the Galaxy Cluster Outer Regions research project.

## Directory Structure

### Data Organization

```
data/
├── raw/                  # Original, unmodified data
│   ├── optical/          # Optical observations
│   ├── xray/             # X-ray observations
│   └── sz/               # Sunyaev-Zel'dovich data
├── processed/            # Processed data products
│   ├── profiles/         # Radial profiles
│   ├── maps/             # Processed 2D maps
│   └── catalogs/         # Source catalogs
└── external/             # External datasets
    ├── simulations/      # Simulation data
    └── literature/       # Published data from papers
```

## Naming Conventions

### Files
- Use lowercase with underscores (snake_case)
- Include date in YYYYMMDD format at the beginning
- Include a descriptive name
- Include version number if applicable
- Example: `20230821_abell1334_xray_spectra_v1.fits`

### Variables in Code
- Use descriptive names in snake_case
- Follow astropy/physics conventions for physical quantities
- Example: `gas_temperature_kev`, `electron_density_cm3`

## Data Processing

1. **Raw Data**
   - Never modify original data files
   - Store metadata (e.g., observation logs, headers) alongside data
   
2. **Processed Data**
   - Document all processing steps
   - Include processing parameters in file headers or sidecar files
   - Use standard FITS or HDF5 formats when possible

## Version Control

- **Do NOT commit** large data files to git (>10MB)
- Use Git LFS for moderately sized data files that need versioning
- For large datasets:
  - Store on institutional storage
  - Create a `data/README.md` with download instructions
  - Include checksums for verification

## Backup Strategy

1. **Critical Data** (raw observations, final results)
   - Store in at least two physical locations
   - Regular backups (daily/weekly)
   
2. **Processing Outputs**
   - Store processing scripts and parameters
   - Document data processing steps
   - Backup final processed data products

## Data Sharing

- Use institutional repositories for long-term storage
- Include README files with metadata
- Follow FAIR principles (Findable, Accessible, Interoperable, Reusable)
- Consider publishing data in relevant archives (e.g., Zenodo, NASA/HEASARC)

## Recommended Tools

- **FITS Handling**: astropy.io.fits, ccdproc
- **Large Datasets**: dask, h5py
- **Versioning**: git-annex, DVC
- **Documentation**: Jupyter notebooks, markdown

## Data Processing Log

Keep a log of all data processing steps in `data/processing_log.md` with entries like:

```markdown
## 2023-08-21: Initial X-ray Data Reduction
- Data: 2023_abell1334_xray_obs1.fits
- Processing:
  - Cleaned for flares
  - Point sources removed
  - Background subtracted
- Output: 20230821_abell1334_xray_clean.fits
- Performed by: [Your Name]
```
