## How to run the simulations  
This Readme file provides the users with the step-by-step guide to successfully run the three developed notebooks.  
The steps, in the order they need to be taken, are explained in what follows.

### STEP_0 Preliminary step  
In this step the modellers make sure that they have access to the content files of the resource and required compute platform.  
 - In order to be able to run the three Jupyter notebooks, modelers need to first have a HydroShare account.  
 - If the modeler already does not have access to CyberGIS-Jupyter for Water (CJW), they need to ask to get access to it at [the CyberGIS-Jupyter for Water platform](https://www.hydroshare.org/group/157)  


**Important notes before running the notebooks**:  
 - Users can change the HRU ID and simulation periods to analyze any of the 671 basins in CAMELS datasets for the simulation period of their choice.  
 - To run each notebook:  
	1. Click the OpenWith button in the upper-right corner of this HydroShare resource webpage;  
	2. Select "CyberGIS-Jupyter for Water";  
	3. Open the notebook and follow instructions;  

### STEP_1 Create SUMMA input using 1_camels_make_input.ipynb
The first notebook creates SUMMA input using Camels dataset using `summa_camels_hydroshare.zip` in this resource and [OpenDAP resource](https://www.hydroshare.org/resource/a28685d2dd584fe5885fc368cb76ff2a/).  

### STEP_2 Execute SUMMA using 2_camels_pysumma.ipynb
This notebook executes SUMMA using original and constant forcing, and different parameters and parameterization combinations.  

### STEP_3 Visualize SUMMA output using 3_camels_analyze_output.ipynb
The final notebook visualizes the sensitivity of SUMMA output according to the constant forcing and output variables using KGE (Kling-Gupta Efficiency).  

