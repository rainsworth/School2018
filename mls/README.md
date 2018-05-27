# Machine Learning and Statistics

## Recommended Python Environment

The notebooks on Machine Learning and Statistics have been developed and tested with the following standalone conda environment. You are encouraged to create the same environment for working with these notebooks.

1. Create a new environment by entering (or pasting) the following command at a shell prompt. **You may need to scroll right to see the whole line, which ends with "pillow".**
```
conda create -n Asterics2018MLS python=3.6 pip ipython jupyter numpy scipy pandas matplotlib seaborn scikit-learn hdf5 pytables pillow
```
2. Activate the new environment using (this should add "(Asterics2018MLS)" to your command prompt, as a reminder of your current environment):
```
source activate Asterics2018MLS
```
3. Add some additional packages that are not included in the base conda distribution:
```
conda install -c astropy emcee astroml
pip install wpca autograd tensorflow edward
```

You only need to complete steps 1-3 once. This new environment will not interfere with your base conda environment or any other custom environments. To revert to your original conda environment at any time, use:
```
source deactivate
```
To return to this environment again, use step 2.

In case something goes wrong with your installation and you want to start again, or if you want to remove this environment after the course, shutdown any active jupyter sessions then use:
```
conda remove --name Asterics2018MLS --all
```

**Windows users:** Your activate/deactivate commands are slightly different. See [here](https://conda.io/docs/user-guide/tasks/manage-environments.html#activating-an-environment) for details.
