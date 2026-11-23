# Can structure-based docking identify FDA-approved drugs that bind PPARδ like GW501516?

AS.410.662 Molecular Modeling for Drug Discovery, Fall 2026. Chris Head.

## What this is
AutoDock Vina screen of 109 acid-containing FDA-approved drugs against
PPARδ (PDB 5U46), benchmarked against 57 known PPARδ actives from ChEMBL 37.

## Results
- Redock validation: GW501516, 3 seeds, RMSD 0.83 / 0.88 / 0.85 Å
- ROC AUC 0.892 over the full set
- Size-controlled (MW 400–600, n=96): MW alone 0.605, docking 0.824

## Running it
Open `notebook.ipynb` in Google Colab on a CPU runtime and run top to bottom.
The first cell downloads the two input files from this repository.

**A full run takes about five hours**, nearly all of it docking. Every output
is included here, so any number in the manuscript can be checked without
re-running the screen.

Package versions: `requirements.txt`.

## Data
ChEMBL release 37, used under CC BY-SA 3.0.
Structure: RCSB PDB 5U46. GW501516: PubChem CID 9803963.
