# Structural MRI: CAT12 vs FreeSurfer (OASIS-1)

**Goal (1–2 lines):** Do CAT12 and FreeSurfer produce comparable morphometry (e.g., cortical thickness/volumes) on a small OASIS-1 subset?

---

## Snapshot
- **Dataset:** OASIS-1 (T1 MRI) — small subject subset
- **Local subset:** <N subjects>  · **Disk:** keep ≤ ~2–5 GB (start with 1–2 subjects)
- **Tools:** SPM12 + CAT12, FreeSurfer
- **Status:** <planned / in progress / complete>
- **Last updated:** <YYYY-MM-DD>

---

## Data
- **Source & license:** Link to OASIS-1 page and note license/DUA.
- **What I downloaded:** list subject IDs; explain why this subset.
- **Layout:** BIDS if available; otherwise keep a simple folder structure.

---

## Pipeline (high-level)
1) CAT12 segmentation / surface processing  
2) FreeSurfer `recon-all`  
3) ROI extraction (Desikan/Destrieux) and CAT12 ROI table  
4) Compare CAT12 vs FreeSurfer (scatter/ICC)  
5) QC: CAT12 report + FS logs/screenshots

---

## Results (to be filled)
- Figure 1: CAT12 vs FS thickness (ROI scatter)  
- Table 1: ROI differences / ICC  
- Notes: potential biases (e.g., smoothing, skull-strip differences)

---

## Reproducibility
- Versions in `env/TOOL_VERSIONS.md`.  
- Steps to rerun (short): “Install SPM/CAT12 & FreeSurfer → place T1s → run CAT12 → run FS → export ROIs → compare.”
- Limitations: tiny N, scanner/site heterogeneity.

---

**Author:** Rene Andrade Rey · 🧪 ORCID: https://orcid.org/0000-0001-5627-579X · 🌐 Scholar: https://scholar.google.es/citations?hl=es&user=Nl3ApFEAAAAJ
