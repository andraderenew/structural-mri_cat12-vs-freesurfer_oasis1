# Structural MRI — CAT12 vs FreeSurfer (OASIS-1)
[![License](https://img.shields.io/github/license/andraderenew/structural-mri_cat12-vs-freesurfer_oasis1)](LICENSE)
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.XXXXXXX-blue)](#cite-this-work)
[![Pages](https://img.shields.io/website?url=https%3A%2F%2Fandraderenew.github.io%2Fstructural-mri_cat12-vs-freesurfer_oasis1%2F)](https://andraderenew.github.io/structural-mri_cat12-vs-freesurfer_oasis1/)
![Release](https://img.shields.io/github/v/release/andraderenew/structural-mri_cat12-vs-freesurfer_oasis1?include_prereleases)
![Last commit](https://img.shields.io/github/last-commit/andraderenew/structural-mri_cat12-vs-freesurfer_oasis1)
[![ORCID](https://img.shields.io/badge/ORCID-0000--0001--5627--579X-A6CE39)](https://orcid.org/0000-0001-5627-579X)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Profile-4285F4)](https://scholar.google.es/citations?hl=es&user=Nl3ApFEAAAAJ)

**One-line:** Morphometry agreement between CAT12 and FreeSurfer on a tiny OASIS-1 subset with QC and ROI summaries.

## Overview
Compare cortical thickness/volumes between **CAT12 (SPM)** and **FreeSurfer** on a tiny **OASIS-1** subset. Include quick QC, ROI tables, and a short agreement analysis (scatter/ICC).

## Data & subset
See `DATA_SOURCES.md`. Working subset: <2–5 subjects> to keep disk ≤ ~5–8 GB including derivatives.

## Pipeline
CAT12 surface/morphometry → FreeSurfer `recon-all` → ROI export (Desikan/Destrieux) → compare & plots → QC (CAT12 report + FS logs).

## Results (to be filled)
- ROI scatter plots (CAT12 vs FS thickness/volume)  
- ICC table and Bland–Altman (optional)  
- QC notes (failed surfaces, skull-strip differences)

## Reproducibility
- Versions: see `env/TOOL_VERSIONS.md`  
- Steps: “Run CAT12 → run FreeSurfer → export ROIs → compare → figures.”  
- Limits: tiny N; scanner/site heterogeneity

## Cite this work
A `CITATION.cff` is included; GitHub shows a “Cite this repository” box. Add DOI after your first Zenodo-backed Release.
