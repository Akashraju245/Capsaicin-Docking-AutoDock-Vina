Capsaicin Molecular Docking using AutoDock Vina
This project focuses on predicting potential protein targets of Capsaicin using SwissTargetPrediction and performing molecular docking analysis using AutoDock Vina.

Project Overview
Capsaicin is a bioactive compound known for its anti-inflammatory and pharmacological properties. In this study, molecular docking was performed to analyze the interaction between Capsaicin and the target protein.

Tools Used
- SwissTargetPrediction
- AutoDock Vina
- PyMOL
- Protein Data Bank (PDB)

Workflow

1. Ligand Preparation
 - Capsaicin structure obtained from PubChem
 - Converted to MOL2 format
 - Prepared ligand file for docking

2. Protein Preparation
  - Protein downloaded from Protein Data Bank
  - Cleaned and modified structure
  - Converted to PDBQT format

3. Docking
 - Docking performed using AutoDock Vina
 - Parameters defined in configuration file
 - Binding poses generated

4. Visualization
 - Docked complex visualized in PyMOL
 - Binding interactions analyze
 - Project Structure

protein/
Contains prepared protein structure

ligand/
Contains ligand files used for docking

docking_results/
Contains docking output files

parameters/
Docking configuration parameters

Results
The docking results indicate potential binding interactions between Capsaicin and the selected protein target.
