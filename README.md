# Drug-Discovery

Majority of the codes and works are inspired by https://projects.volkamerlab.org/teachopencadd/talktorials and https://github.com/Ash100.

Tut001_Compound_Data_Acquisition_(ChEMBL).ipynb used V5TFZ2 (Uniprot ID; https://www.uniprot.org/uniprotkb/V5TFZ2/entry) which is infact Dengue Type-2 NS5 protein.

Tut002_Dataset_Filteration_and_Analysis.ipynb uses the file "NS5_compounds.csv" produced in Tut001. This file (NS5_compounds.csv) is also present in this folder.



Step          Known Ligands (ChEMBL, labeled)            Unknown Ligands (ZINC, unlabeled)
T001          Query ChEMBL for Dengue NS3 bioactivity data (IC₅₀, pIC₅₀).          Not applicable yet — we start with ChEMBL to build the training set.
T002
Apply Lipinski’s Rule of Five filters.
Apply same filters to ZINC when you load them later (consistency).
T003
Remove PAINS, undesirable chemotypes, duplicates.
Apply identical cleaning/PAINS removal to ZINC set.
T004
Generate fingerprints/features for known ligands.
Generate exact same type of features for ZINC molecules.
T005
Cluster known ligands to inspect chemical diversity.
Optionally cluster ZINC hits after scoring to get diverse hits.
T006
Find Maximum Common Substructure (MCS) among known actives.
Apply MCS to predicted ZINC hits to understand core scaffolds.
T007
Train & validate ML classifier (active/inactive) using known ligands.
Apply the trained ML model to ZINC to predict activities.
T008
Prepare protein structure for docking known actives.
Dock top-predicted ZINC hits into EGFR structure.
T009
Define docking binding site from known ligand poses.
Same binding site is used to dock predicted ZINC hits.
T010
Run docking on known ligands as benchmark.
Run docking on ZINC hits to refine predictions.
T011
Visualize docking poses for known ligands.
Visualize poses of ZINC hits and compare to known actives.
T012
Evaluate docking scores & interaction patterns for known ligands.
Evaluate docking scores & interaction patterns for ZINC hits.
T013
Create final hit list from validated known ligands (optional).
Select top ZINC candidates for experimental testing.
