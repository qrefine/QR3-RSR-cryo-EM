# QR3-RSR-cryo-EM
Re-refinement results from Real-space quantum-based refinement for cryo-EM: Q|R#3

1. Atomic models and corresponding maps have been selected from the Protein Data Bank and Electron Microscopy Data Bank. 
The 3a5x model was used as is, while only chains A and C were used from 3j63 and 5fn5, respectively. Each model was subject to a fully automated preparation for quantum refinement using the qr.finalise tool of the Q|R package; this includes completing missing side chains and adding all theoretically possible (but missing) hydrogen atoms. For partial models (3j63 and 5fn5) a box with the map around corresponding chains was extracted using the phenix.map_box tool. Such prepared models and maps have been used in all refinements and are provided in start_pdbs and EM_maps directories.

2. All refinements were performed using qr.refine. Quantum refinement was performed using the TeraChem and xtb packages as QM engines, with the HF-D3/61G and GFN1-xTB as quantum models. Classic refinement (CCTBX refinement) used geometry restraints as implemented in CCTBX.
The commands used in qr.refine (command*), re-refined pdbs (*.pdb) and outputs of refinement runs (*log) are provided.

