# 27032 Introduction to cell factories -- metabolic modeling practical

Colab notebooks for the metabolic modeling session of DTU course **27032
"Introduction to cell factories"**. You will load a genome-scale metabolic model with
[cobrapy](https://cobrapy.readthedocs.io), set its bounds from real numbers, run flux
balance analysis (FBA) and flux variability analysis (FVA), and then do the same on a
model of your choice. Click a badge to open a notebook in Google Colab -- nothing to
install. Run the first cell of every notebook before anything else.

| notebook | what it covers | open |
|---|---|---|
| `00_check_setup` | does my environment work? (under a minute) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BRIGHT-CDA/27032-metabolic-modeling/blob/main/notebooks/00_check_setup.ipynb) |
| `01_fba_basics` | load and inspect a model, set bounds, FBA, FVA, then your own model | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BRIGHT-CDA/27032-metabolic-modeling/blob/main/notebooks/01_fba_basics.ipynb) |
| `02_growth_coupling` | production envelope, growth coupling by knockouts | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BRIGHT-CDA/27032-metabolic-modeling/blob/main/notebooks/02_growth_coupling.ipynb) |

Colab opens a copy that only you can see. To keep your work, use **File > Save a
copy in Drive**.

## If Colab doesn't work for you

The same notebooks run on your own machine. Install
[Miniforge](https://github.com/conda-forge/miniforge) (or any conda), download this
repository, and from its folder run:

```bash
conda env create -f environment.yml
conda activate 27032-metabolic-modeling
jupyter lab
```

Then open the notebooks from the `notebooks/` folder. The setup cell detects that it
is not in Colab and finds everything already installed. Escher (flux maps) is
optional: if it gives you trouble, everything else still works.
