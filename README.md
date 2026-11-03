# APS Python Introduction

This is a simple example of how to control the APS environment using python.  
More detailed examples of how to connect to APS can be found in the ScriptingInterface_2024 folder.  


## Setting up your development environment  
* Install MiniForge https://github.com/conda-forge/miniforge?tab=readme-ov-file
* install vscode https://code.visualstudio.com/ and extensions  ms-python.vscode-pylance, ms-python.python, ms-toolsai.jupyter
* (Optional) install gitbash https://git-scm.com/download/win
* (Optional) Set up [ssh keys using git bash](https://docs.oracle.com/en/cloud/cloud-at-customer/occ-get-started/generate-ssh-key-pair.html#GUID-8B9E7FCB-CEA3-4FB3-BF1A-FD3406A2432F) 


## Set up ENV
These are the steps to get started:
1. Navigate to project folder and run the command below to the create conda environment which reads the environment.yml file.
2. Create the virtual environment using conda and poetry. The basic commands are as follows:   
    ``` conda env create ```  
    * Activate the virtual environment  with
    ```conda activate aps-env```
    * Install the packages using poetry (retry if it fails)
    ``` poetry install -vvv  ```
    * To update the packages 
   ``` poetry update ```
    * To remove the env
   ``` conda env remove --name aps-env ```
   * The interpreter path can be found by tying  ```which python```
   * Append the project's virtual env to the jupyter kernels
   ``` python -m ipykernel install --user --name aps-env --display-name "aps-env" ```

## Run the notebook

1. Ensure that APS simulation is opened in APS
2. Open the notebook and select the aps-env environment before running the notebook 



