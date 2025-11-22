## Overview
Compare cortical thickness/volumes between **CAT12 (SPM)** and **FreeSurfer** on a tiny **OASIS-1** subset. Include quick QC, ROI tables, and a short agreement analysis (scatter/ICC).

## Data & subset
See `DATA_SOURCES.md`. Working subset: <2–5 subjects> to keep disk ≤ ~5–8 GB including derivatives.

## Pipeline
CAT12 surface/morphometry → FreeSurfer `recon-all` → ROI export (Desikan/Destrieux) → compare & plots → QC (CAT12 report + FS logs).
# neuro-project-template
