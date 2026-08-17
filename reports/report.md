# Cross-Method Structural MRI Report

## Aim

Document a descriptive single-subject comparison between CAT26/SPM25 and FreeSurfer using the same public T1-weighted MRI from OpenNeuro `ds000114`.

## Data

- Participant: `sub-01`
- Session: `ses-test`
- Structural image: `sub-01_ses-test_T1w.nii`

## Source methods

### CAT26 / SPM25

The validated CAT source project used MATLAB R2025b, SPM25 `25.01.02`, and CAT26 `26.0.rc3` (build 3250). Public outputs include global GM, WM, CSF and TIV summaries plus CAT image-quality metrics and QC figures.

### FreeSurfer

The validated FreeSurfer source project used FreeSurfer 7.4.1. Public outputs include global and subcortical volumes, bilateral Desikan-Killiany cortical thickness, surface area and cortical volume tables, reconstruction logs, topology validation, and QC figures.

## Comparison status

The two source pipelines are complete and independently audited. This repository does not currently claim a completed region-by-region CAT26-versus-FreeSurfer agreement analysis because directly harmonized CAT regional outputs are not retained here.

Any quantitative cross-method comparison must first verify that the selected measures have compatible anatomical definitions and units. Single-subject data are not sufficient for ICC or population-level agreement inference.

## QC

QC evidence is retained in the respective source repositories. Both pipelines were visually reviewed during their individual repository audits.

## Limitations

- one participant only
- software-specific anatomical definitions and measurement conventions
- CAT26 and FreeSurfer cortical/subcortical outputs are not automatically interchangeable
- no population inference or diagnostic interpretation

## Reproducibility

See `README.md`, `DATA_SOURCES.md`, and `env/TOOL_VERSIONS.md`, together with the two validated source repositories.
