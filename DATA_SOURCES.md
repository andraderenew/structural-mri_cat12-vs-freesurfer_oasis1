# Data Sources

## Primary dataset

- Repository: OpenNeuro
- Dataset: `ds000114`
- Participant: `sub-01`
- Session: `ses-test`
- Modality: T1-weighted structural MRI
- Input file: `sub-01_ses-test_T1w.nii`

The same public T1-weighted image was used by both validated source pipelines that this comparison coordinates.

## Source processing repositories

- CAT26/SPM25: `andraderenew/structural-mri_cat12_single_subject`
- FreeSurfer: `andraderenew/structural-mri_freesurfer_single_subject`

The CAT repository name is historical; the completed analysis used CAT26 with SPM25.

## Data handling

Raw MRI data and large derivative workspaces are excluded from this repository. Public comparison material should contain only portable scripts, documentation, summary tables, figures, and provenance needed to understand or reproduce the comparison from the source pipelines.
