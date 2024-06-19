[UNDER DEVELOPMENT - CHECK BACK IN A FEW WEEKS]
# Plotting Your Course with Effective Data Exploration

## Workshop Description
In data science, much of the conversation often revolves around the sophistication of models. While good model archetecture is important, the conversation seldom dives deep into the pivotal role of data exploration in enhancing our analytical workflow. This workshop aims to shift the focus to the underappreciated yet exciting process of data exploration, I will be walking you through steps you can take to gain intuition about your data, so you can ask the right questions, generate hypothesis, and create the _right_ model. 

## Goals and Expectations
By the end of this workshop, participants will be equipped with the knowledge and skills to conduct thorough data explorations, laying a solid foundation for any subsequent machine learning or data analysis projects. You'll leave with a deeper appreciation for the art of data exploration and a set of practical tools and techniques to apply to real-world datasets.
* Encourage Intuition Building: Provide workflows for participants to help gain deep insights and intuition about their data, transforming raw numbers into narratives threads that can be explored.
* Practical Skillset: Move beyond theoretical knowledge so attendees can leave with practical approaches and strategies for data exploration.
* Stoke Curiosity: Help participants see data exploration as a exciting steps and shift attitudes from accepting data at face value to actively questioning and probing data to uncover underlying issues, patterns, anomalies, and trends.

## Setup Documentation
1. Folder and Files
INPUTS: Input data of watershed characteristics is not included in this repository.
    - Water table depth (annual means) from [Fan, Y. et al. (2013)](doi.org/10.1126/science.1229881)
    - Dataset1_BasinID, Dataset5_LandUse, Dataset6_N-P_Fertilizer-Manure, [Falcone, J. A. (2017a)](doi.org/10.5066/F7TX3CKP)
    - Dataset19_PointSource, Dataset24_Static, [Falcone, J. A (2017b).](doi.org/10.5066/F7HQ3XS4)
    - Dataset99_TileDrainage [Valayamkunnath, P. et a. (2020)](doi.org/10.1038/s41597-020-00596-x)
    - Dataset99_AridityIndex [Zomer, R., & Trabucco, A. (2022)](doi.org/10.6084/M9.FIGSHARE.7504448.V6)
CODE: Jupyter notebooks create for downloading data and processing data.
- DATA_datasetCompilation.ipynb for downloading water flow and concentration data.
OUTPUT: folders for generated files. 
environment_*.yaml: conda environment config file.

2. Software
To setup the environment, please install conda (Anaconda or miniconda) first, then create env via the config yaml.

conda env create --file dataExploration.yaml --name dataExploration
conda activate dataExploration

3. Extra dataset download
I use two additional dataset, 'Falcone, J.A., 2017. USGS Data Release. https://doi.org/10.5066/F7HQ3XS4' and XXX. 