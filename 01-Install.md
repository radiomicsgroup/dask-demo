# Install

Create a conda environment

```bash
conda create -n dask python=3.8.5
conda activate dask
pip install readline  pyzmq graphviz jupyter ipykernel notebook  jupyterlab  jupyter_contrib_nbextensions

conda install dask -c conda-forge or pip install dask[complete]

conda install  -c conda-forge jupyter ipykernel notebook nb_conda_kernels jupyterlab nb_conda_kernels  jupyter_contrib_nbextensions pip
```

Remove conda enviroment

```bash
conda env remove -n dask
```
