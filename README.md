# DBGNN_paper-companion

This repository contains the code to reproduce the results of the paper: "Dirac--Bianconi Graph Neural Networks -- Enabling Non-Diffusive Long-Range Graph Predictions". The repository contains code to train ML models and to make the trajectory plots. The full code for generating the figures and the trained models can be found on Zenodo: ihttps://doi.org/10.5281/zenodo.12687981. 

## Training of the ML models
```
conda env create -n py310ptg --file py310ptg.yml
```
The file conda_environment.yml is stored in training_model.

The following parameters need to be set in ```start_ray.py```:
```
dataset_path = Path(PATHMISSING)
dataset_path = Path(PATHMISSING)
tmp_dir = "TMP_PATH"
```

Afterward, the script ```start_ray.py``` can be executed.


## Trajectories
The language Julia needs to be installed to generate the plots. First, the package needs to be activated and instantiated. Afterward, the plots can be generated by executing ```julia generate_publication_figures.jl```.  

In case of any problems or questions, do not hesitate to contact us.
