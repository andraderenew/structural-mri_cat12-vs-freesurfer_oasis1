# Structural MRI — CAT26 vs FreeSurfer (OpenNeuro ds000114)

[![License](https://img.shields.io/github/license/andraderenew/structural-mri_cat26-vs-freesurfer_openneuro-ds000114)](LICENSE)
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.17715121-blue)](https://doi.org/10.5281/zenodo.17715121)
![Release](https://img.shields.io/github/v/release/andraderenew/structural-mri_cat26-vs-freesurfer_openneuro-ds000114?include_prereleases)
![Last commit](https://img.shields.io/github/last-commit/andraderenew/structural-mri_cat26-vs-freesurfer_openneuro-ds000114)
[![ORCID](https://img.shields.io/badge/ORCID-0000--0001--5627--579X-A6CE39)](https://orcid.org/0000-0001-5627-579X)

Cross-method structural MRI comparison project using the same public T1-weighted image processed independently with CAT26/SPM25 and FreeSurfer.

## Dataset

- Source: OpenNeuro `ds000114`
- Participant: `sub-01`
- Session: `ses-test`
- Modality: T1-weighted structural MRI
- Input: `sub-01_ses-test_T1w.nii`

Raw neuroimaging data are not stored in this repository.

## Source pipelines

The comparison is based on two separately validated single-subject processing projects using the same OpenNeuro image:

- CAT26/SPM25: [`structural-mri_cat12_single_subject`](https://github.com/andraderenew/structural-mri_cat12_single_subject)
- FreeSurfer: [`structural-mri_freesurfer_single_subject`](https://github.com/andraderenew/structural-mri_freesurfer_single_subject)

The CAT repository name is historical; the completed processing documented there used CAT26 `26.0.rc3` with SPM25 `25.01.02`.

## Software represented by the validated source projects

- MATLAB R2025b
- SPM25 `25.01.02`
- CAT26 `26.0.rc3` (build 3250)
- FreeSurfer 7.4.1

The CAT and FreeSurfer pipelines were run in their respective validated environments; see the source repositories for exact platform and provenance details.

## Comparison scope

The intended comparison is methodological and descriptive. It evaluates how two structural MRI processing frameworks summarize the same anatomy while respecting that their tissue definitions, cortical models, atlases, and derived measures are not interchangeable.

Current public source outputs support:

- CAT global GM, WM, CSF and TIV summaries plus CAT image-quality metrics
- FreeSurfer global/subcortical volumes and Desikan-Killiany cortical thickness, area and volume tables
- independently reviewed QC figures from both source pipelines

A regional CAT-versus-FreeSurfer agreement analysis is not claimed unless directly comparable CAT regional outputs are available and explicitly harmonized.

## Reproducibility

This repository coordinates the cross-method comparison. The executable processing workflows and validated outputs remain in the two source repositories above. Software provenance is summarized in `env/TOOL_VERSIONS.md` and the common data source in `DATA_SOURCES.md`.

## Interpretation

This is a single-subject technical comparison. It does not provide population inference, normative interpretation, diagnostic classification, or evidence that similarly named measures from CAT26 and FreeSurfer are numerically equivalent.

## Author

Rene Andrade Rey  
ORCID: `0000-0001-5627-579X`
