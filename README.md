This repository hosts a Jupyter notebook for running RFdiffusion (v1.1.1) on Google Colab, enabling protein structure generation and design. RFdiffusion, detailed in its bioRxiv manuscript, supports tasks like unconditional generation, binder design, motif scaffolding, partial diffusion, and symmetry-constrained designs.

Features





Sets up RFdiffusion in ~3 minutes with GPU support.



Generates monomers (e.g., 100-residue proteins), hetero-oligomers, or homo-oligomers.



Designs binders to PDB targets with optional hotspot residues.



Supports motif scaffolding and partial diffusion.



Offers visualization: static images or interactive 3D models.

Getting Started





Open diffusion.ipynb in Google Colab (File > Upload Notebook).



Run cells sequentially to install dependencies and RFdiffusion.



Customize parameters (contigs, pdb, hotspot, etc.) in the "run RFdiffusion" cell.



View and download results as a ZIP archive.

Example Usage





Unconditional: contigs='100' for a 100-residue monomer.



Binder Design: contigs='A:50' pdb='4N5T' for a 50-residue binder to chain A.



Motif Scaffolding: contigs='40/A163-181/40' pdb='5TPN' for a motif with flanking regions.



Symmetry: contigs='50' symmetry='cyclic' order=2 for homo-oligomers.

Requirements





Google Colab with GPU runtime (set in Runtime > Change runtime type).



No local installation needed; all dependencies are downloaded in the notebook.

Notes





Check the notebook's markdown cells for detailed instructions.



Outputs include PDB files and trajectories, viewable in tools like PyMOL.



Based on ColabDesign.

