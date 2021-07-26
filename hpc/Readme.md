## How to run the simulations  
This Readme file provides the users with the step-by-step guide to successfully run the three developed notebooks.  
The steps, in the order they need to be taken, are explained in what follows.

### STEP_0 Preliminary step  
In this step the modellers make sure that they have access to the content files of the resource and required compute platform.  
 - In order to be able to run the three Jupyter notebooks, modelers need to first have a HydroShare account.  
 
 - If the modeler already does not have access to CyberGIS-Jupyter for Water (CJW), they need to ask to get access to it at [the CyberGIS-Jupyter for Water platform](https://www.hydroshare.org/group/157)  
    * For the resource, choose open with "CyberGIS-Jupyter for Water"in the dropdown menu on the right side of the resource. 

 - If instead the modeler is choosing to run locally, they will need to download the resource and set up a conda environment and install pysumma:
    * Get an Anaconda Python environment set up and install the environment there as follows;
        1. Check the operating system;
        `cd /path/to/home`;
        `uname -m`;
       2. Get Miniconda for that system. For Linux 64 the command is:
        `wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh`;
        `chmod 777 Miniconda3-latest-Linux-x86_64.sh`;
        `./Miniconda3-latest-Linux-x86_64.sh`;
        3. Close and then re-open your terminal window then iinstall the environment with conda the extra packages, with commands:
        `conda env create -n pysumma -f environment.yml`;
        4. This will make a python environment that you can activate and deactivate as:
        `conda activate pysumma`
        *Install it as a kernel in your Jupyter environments:
        `python -m ipykernel install --user --name=pysumma`;


**Important notes before running the notebooks**:  
 - Users can change the HRU ID and simulation periods to analyze any of the 671 basins in CAMELS datasets for the simulation period of their choice.  
 - To run each notebook:  
    1. Click the OpenWith button in the upper-right corner of this HydroShare resource webpage;  
    2. Select "CyberGIS-Jupyter for Water";  
    3. Open the notebook and follow instructions;  

### STEP_1 Create SUMMA input using 1_camels_make_input.ipynb
The first notebook creates SUMMA input using Camels dataset using `summa_camels_hydroshare.zip` in this resource and [OpenDAP resource](https://www.hydroshare.org/resource/a28685d2dd584fe5885fc368cb76ff2a/).  

### STEP_2 Execute SUMMA using 2_camels_pysumma_hpc.ipynb
This notebook executes SUMMA using original and constant forcing, and different parameters and parameterization combinations via HPC (XSEDE).  

### STEP_3 Visualize SUMMA output using 3_camels_analyze_output.ipynb
This notebook visualizes the sensitivity of SUMMA output according to the constant forcing and output variables using KGE.

### STEP_4 Download raw SUMMA output
