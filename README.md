# auto_ml_exploration
Exploration of Ludwig and PyCaret Frameworks for AutoML

### Repository and Environment Set Up
To create the environment required, perform the following:
```
conda create --name auto_ml python=3.10;
conda activate auto_ml;
pip3 install pycaret ludwig;
pip3 install 'ludwig[viz]';
pip3 install 'ludwig[hyperopt]';
pip3 install dask;
```

Data from I-SPY2 was downloaded and prepared with the help of Jeremy Goecks' 
repository [here](https://github.com/goeckslab/Ludwig-ISPY2/)

Additioinally, datasets were generated with the help of the Ludwig API:
```
ludwig datasets download mnist;
ludwig datasets download irony:
ludwig datasets download mushroom_edibility;
```

In order to utilize the Jupyter notebooks in this repository, make sure to have 
`nb_conda_kernels` installed in your base enviornment, and `ipykernel` 
installed in the development environmnts:
```
conda deactivate;
conda install nb_conda_kernels;
conda activate auto_ml;
conda install ipykernel;
```
