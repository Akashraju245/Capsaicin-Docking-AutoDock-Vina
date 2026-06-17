# Capsaicin Molecular Docking using AutoDock Vina

## Overview
This project investigates the binding potential of Capsaicin — a bioactive 
compound found in chili peppers with known anti-inflammatory and analgesic 
properties — against a protein target identified via SwissTargetPrediction. 
Molecular docking was performed using AutoDock Vina, and binding poses were 
visualized in PyMOL.

## Tools & Technologies
- SwissTargetPrediction — target identification
- AutoDock Vina — molecular docking
- PyMOL — 3D visualization of binding interactions
- Protein Data Bank (PDB) — protein structure source
- PubChem — ligand structure source

## Workflow
1. Retrieved Capsaicin SMILES from PubChem; converted to MOL2 and PDBQT format
2. Identified top protein targets using SwissTargetPrediction
3. Downloaded target protein (PDB ID: 7LR0) and prepared structure (removed 
   water molecules, added polar hydrogens)
4. Defined docking grid box around the active site
5. Ran molecular docking using AutoDock Vina with defined parameters
6. Visualized top binding pose and interactions in PyMOL

## Key Results
- Target protein: 7LR0 (TRPV1 — Transient Receptor Potential Vanilloid 1), 
  a well-known receptor for Capsaicin
- Docking performed and binding poses generated
- Best binding pose visualized using PyMOL showing ligand placement within 
  the active site

## Files in This Repository
| File | Description |
|------|-------------|
| `7lr0_modified.pdb` | Prepared protein structure |
| `ligand.pdbqt` | Capsaicin ligand file for docking |
| `system.pdbqt` | Receptor file for docking |
| `vina_dock.pdbqt` | Docking output with binding poses |
| `parameters` | AutoDock Vina configuration file |

## Limitations & Future Work
- Binding energy values to be updated after full AutoDock Vina run
- Future: run MD simulation to validate docking stability
- Expand to screen multiple Capsaicin analogues

## References
- AutoDock Vina: https://vina.scripps.edu
- SwissTargetPrediction: http://www.swisstargetprediction.ch
- RCSB PDB: https://www.rcsb.org
