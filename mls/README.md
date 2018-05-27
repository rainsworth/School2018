# Machine Learning and Statistics

## Recommended Python Environment

The notebooks on Machine Learning nd Statistics have been developed and tested with the following standalone conda environment. You are encouraged to create the same environment for working with these notebooks.

1. Create a new environment by entering (or pasting) the following command at a shell prompt. *Enter the command on one line*, even though it appears on two lines below:
```
conda create -n MLS python=3.6 pip ipython jupyter numpy scipy pandas
    matplotlib seaborn scikit-learn hdf5 pytables pillow
```
2. Activate the new environment using (this should add "(MLS)" to your command prompt, as a reminder of your current environment):
```
source activate MLS
```
*Windows users:* Wherever you see `source activate MLS`, use `activate MLS` instead. Details [here](https://conda.io/docs/user-guide/tasks/manage-environments.html#activating-an-environment).
3. Add some additional packages that are not included in the base conda distribution:
```
conda install -c astropy emcee astroml
pip install wpca autograd tensorflow edward
```

In case something goes wrong with your installation and you want to start again, use:
```
conda remove --name MLS --all
```
You will need to shutdown any jupyter sessions with the old environment first.
