# Data Directory

This folder contains data used in the Galaxy Cluster Outer Regions project.

- `raw/`: Original, unmodified datasets (optical, X-ray, SZ)
- `processed/`: Data products derived from processing/analysis
- `external/`: Reference datasets from literature or simulations

Large files should not be committed directly unless tracked with Git LFS.

## Access and Storage
- Primary storage: [describe institutional path or bucket]
- Backup location: [describe backup]
- Retrieval instructions: [e.g., command lines, credentials handling]

## Dataset Catalog
Provide a short entry for each dataset:

```
- Name: Planck y-map (PR3)
  Location: data/external/planck_pr3/
  Source: https://pla.esac.esa.int
  Version: PR3
  Notes: used for SZ profiles

- Name: Chandra ObsID 12345 (Cluster XYZ)
  Location: data/raw/xray/chandra/ObsID_12345/
  Source: HEASARC
  Notes: see docs/processing_log.md for reduction details
```

## Checksums
Include checksums for critical files in a `CHECKSUMS.txt` (e.g., sha256) to verify integrity.
