# Tool Versions and Provenance

## CAT26 / SPM25 source pipeline

- MATLAB: R2025b
- SPM: 25.01.02
- CAT: 26.0.rc3 (build 3250)
- Platform: macOS, Apple Silicon
- MATLAB architecture: `maca64`

These values are taken from the completed `structural-mri_cat12_single_subject` project. Its repository name is historical; the documented processing used CAT26, not CAT12.

## FreeSurfer source pipeline

- FreeSurfer: 7.4.1
- Platform: Ubuntu 22.04.5 LTS
- OpenMP threads used for the validated reconstruction: 8

These values are taken from the completed `structural-mri_freesurfer_single_subject` project.

## Comparison provenance

The two source pipelines processed the same OpenNeuro `ds000114` T1-weighted image for `sub-01`, `ses-test`. They were run in different validated environments, so this comparison repository does not imply that the software packages were executed within one shared environment.
