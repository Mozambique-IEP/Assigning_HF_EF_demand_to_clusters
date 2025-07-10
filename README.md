# Assigning Social Demand to Population Clusters

Jupyter notebook that automated the assignment and integration of electricity demand to population clusters. To use this notebook you will need to have the following datasets/layers:
* Administrative boundaries
* Health Facilities database (.csv is fine)
* Education Facilities database (.csv is fine)
* Calibrated Input file for OnSSET

The output is in the form of a CSV file that can be directly put into OnSSET, including demand columns for Health and Education related activity.

## Content
This repository contains:
* The code and related functions. These files also have instructions for how to run the code
* Example input and output files (note that calibrated file as well as updated output are omitted, but can be shared/added with UIPCE's permission)

## Installing and running the extraction notebook

**Requirements**

This module have been developed in Python 3. You are recommended to install [Anaconda's free distribution](https://www.anaconda.com/distribution/) as suited for your operating system. 

**Install the extraction repository from GitHub**

After installing Anaconda you can download the repository directly or clone it to your designated local directory using:

```
> conda install git
> git clone -https://github.com/Mozambique-IEP/Assigning_HF_EF_demand_to_clusters.git
```
Once installed, open anaconda prompt and move to your local "Assigning_HF_EF_demand_to_clusters" directory using:
```
> cd ..\Assigning_HF_EF_demand_to_clusters
```

In order to be able to run the tool you have to install all necessary packages. The code runs on the same environment as the calibration/OnSSET code. That is, if you have already configured the "moz_onsset_env.yml" you should be good to go. Else, use get the .yml file from the other repositories in this organization and run the following:

```
conda env create --name OnSSET_env --file moz_onsset_env.yml
```

This might take some time. When complete, activate the virtual environment using:

```
conda activate OnSSET_env
```

With the environment activated, you can now move to the extraction directory and start a "jupyter notebook" session by simply typing:

```
..\Assigning_HF_EF_demand_to_clusters> jupyter notebook 
```
## Changelog
**10-July-2025**: Original code base published
s
