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
### Folder and Files
INPUTS: Input data of watershed characteristics is not included in this repository.
- Dataset1_BasinID, Dataset5_LandUse, Dataset6_N-P_Fertilizer-Manure ([Falcone, J. A. (2017a)](https://www.sciencebase.gov/catalog/item/631405bbd34e36012efa304a))
- Dataset99_PointSource ([Ivahnenko, T.I. (2017)](https://www.sciencebase.gov/catalog/item/582f41a4e4b04d580bd51af5))
- Dataset99_Slope ([USGS National Elevation Dataset, accesssed 2024](https://rockyweb.usgs.gov/vdelivery/Datasets/Staged/Elevation/1/TIFF/current/))
- Dataset99_AridityIndex ([Zomer, R., & Trabucco, A. (2022)](https://figshare.com/articles/dataset/
Global_Aridity_Index_and_Potential_Evapotranspiration_ET0_Climate_Database_v2/7504448/6))
- Dataset99_DepthGW ([Fan, Y. et al. (2013)](https://www.science.org/doi/10.1126/science.1229881))
- Dataset99_TileDrainage ([Valayamkunnath, P. et a. (2020)](https://www.nature.com/articles/s41597-020-00596-x))

CODE: Jupyter notebooks create for downloading data and processing data.
- DATA_datasetCompilation.ipynb for compiling watershed attributes and downloading water flow and concentration data.

OUTPUT: folders for generated files. 
- environment_*.yaml: conda environment config file.

### Software
To setup the environment, please install conda (Anaconda or miniconda) first, then create env via the config yaml.

conda env create --file dataExploration.yaml --name dataExploration
conda activate dataExploration