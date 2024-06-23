# Plotting Your Course with Effective Data Exploration

## Workshop Description
In data science, much of the conversation often revolves around the sophistication of models. While good model architecture is important, the conversation seldom dives deep into the pivotal role of data exploration in enhancing our analytical workflow. This workshop aims to shift the focus to the underappreciated yet exciting process of data exploration, I will be walking you through steps you can take to gain intuition about your data, so you can ask the right questions, generate hypothesis, and create the _right_ model. 

## Goals and Expectations
By the end of this workshop, participants will be equipped with the knowledge and skills to conduct thorough data explorations, laying a solid foundation for any subsequent machine learning or data analysis projects. You'll leave with a deeper appreciation for the art of data exploration and a set of practical tools and techniques to apply to real-world datasets.
* Encourage Intuition Building: Provide workflows for participants to help gain deep insights and intuition about their data, transforming raw numbers into narratives threads that can be explored.
* Practical Skillset: Move beyond theoretical knowledge so attendees can leave with practical approaches and strategies for data exploration.
* Stoke Curiosity: Help participants see data exploration as a exciting steps and shift attitudes from accepting data at face value to actively questioning and probing data to uncover underlying issues, patterns, anomalies, and trends.

## Setup Documentation
### Folder and Files
INPUTS: Input data of watershed characteristics is not included in this repository. Contents of the INPUTS folder are:
- workshop_DataExploration.yml: virtual environment .yml file. See notes below for import. 
- WtshdAttributeTable_20240603.txt: Watershed attribute data file.
- CQ_Data_20240604.txt: Paired concentration and discharge recording for 2594 watersheds from 1980 to 2020.
- Dataset_XX: Raw watershed attributes input folders each contain a textfile with watershed characteristics. 
- boundaries-shapefiles-by-aggeco/: Folder that contains watershed shapefile.
- cb_2017_us_state_5m/: Folder that contains US state boundary.

CODE: Jupyter notebooks create for downloading data and processing data.
- DATA_datasetCompilation.ipynb compiles watershed attributes and downloading water flow and concentration data. The output of this script is 'WtshdAttributeTable_20240603.txt' and 'CQ_Data_20240604.txt'.
- ANA_dataExploration.ipynb performs the analysis and data exploration of the watershed's concentration-discharge and attribute analysis. 

### Software
To setup the environment, please install conda (Anaconda or miniconda) first, then create env via the config yaml.
Open Anaconda Prompt
Navigate to the location of the .yml file (e.g., INPUTS/).
Run the following commands:
```
conda env create -f workshop_DataExploration.yml
conda activate workshop_DataExploration
```
