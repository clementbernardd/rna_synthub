# Data description

- `examples`: contains the different results with examples
- `img`: fodler with the different visualisation
- `metadata`: 
    - `filter`: folder with the output from the different filtering processes: clash, rnaspider and molprobity. 
        - `meta_scores.csv``: dataframe with the sequence and the different scoring functions computed from the raw Kaggle dataset.
        - `top_meta_scores.csv`: dataframe with the scoring functions from the top 50k structures
    - `results`: folder after applying filtering or clustering
        - `clustered.csv`: obtained cluster after applying locarna
        - `filtered.csv`: obtained dataset before applying locarna
        - `top_50k.csv`: obtained dataframe with top 50K data: scoring functions and filtering steps
- `raw`: folder with the structures from the RNA-SyntHub dataset. It can be downloaded from this [link](https://zenodo.org/records/17222400)
  - `angles`: extracted angles from the raw dataset
  - `distance`: extracted distances from the raw dataset
  - `PDB`: raw PDB structures for the RNA-SyntHub dataset (RFDiffusion, Boltz-1, RNAComposer) 
 and the native dataset used as a comparison. The structures for RNA-SyntHub is in `raw` folder.
We also include predictions from other structures in the `raw_all` folder.
- `times`: folder with the data from times benchmark