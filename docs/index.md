# Structural MRI: CAT26 vs FreeSurfer on OpenNeuro ds000114

## Goal

Compare structural MRI outputs from CAT26/SPM25 and FreeSurfer for the same public T1-weighted image while keeping method-specific definitions and limitations explicit.

## Snapshot

- Dataset: OpenNeuro `ds000114`
- Participant: `sub-01`
- Session: `ses-test`
- Input: `sub-01_ses-test_T1w.nii`
- CAT pipeline: SPM25 `25.01.02` + CAT26 `26.0.rc3` (build 3250)
- FreeSurfer pipeline: FreeSurfer 7.4.1
- Status: source pipelines completed and audited; cross-method comparison repository being aligned to those validated outputs

## Data

Both source projects processed the same OpenNeuro structural MRI. Raw data are excluded from GitHub.

Validated source repositories:

- `andraderenew/structural-mri_cat12_single_subject`
- `andraderenew/structural-mri_freesurfer_single_subject`

The CAT source repository retains a historical name, but its completed processing used CAT26 and SPM25.

## Available source outputs

CAT26/SPM25 provides global tissue volumes and image-quality metrics. FreeSurfer provides global and subcortical volumes plus Desikan-Killiany cortical thickness, surface area, and cortical volume tables. Both projects include reviewed QC figures.

## Comparison principles

1. Compare only measures with defensible semantic correspondence.
2. Do not treat similarly named CAT26 and FreeSurfer outputs as interchangeable by default.
3. Keep single-subject comparisons descriptive.
4. Do not report ICC or population-level agreement statistics from one participant.
5. A regional cross-method analysis requires explicitly harmonized regional outputs from both pipelines.

## Reproducibility

Processing provenance is retained in the two source repositories. This repository documents the common input, cross-method scope, and any comparison outputs produced from those validated source results.

## Limitations

This is a single-subject technical comparison. Differences between software packages can reflect distinct segmentation models, cortical reconstruction procedures, atlas definitions, quality-control procedures, and measurement conventions.

**Author:** Rene Andrade Rey · ORCID: https://orcid.org/0000-0001-5627-579X
