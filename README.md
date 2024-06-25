# Plotting Your Course with Effective Data Exploration

## Workshop Description
In data science, much of the conversation often revolves around the sophistication of models. While good model architecture is important, the conversation seldom dives deep into the pivotal role of data exploration in enhancing our analytical workflow. This workshop aims to shift the focus to the underappreciated yet exciting process of data exploration, I will be walking you through steps you can take to gain intuition about your data, so you can ask the right questions, generate hypotheses, and create the _right_ model. 

## Goals and Expectations
By the end of this workshop, participants will be equipped with the knowledge and skills to conduct thorough data exploration, laying a solid foundation for any subsequent machine learning or data analysis projects. You'll leave with a deeper appreciation for the art of data exploration and a set of practical tools and techniques to apply to real-world datasets.
* Encourage Intuition Building: Provide workflows for participants to help gain deep insights and intuition about their data, transforming raw numbers into narrative threads that can be explored.
* Practical Skillset: Move beyond theoretical knowledge so attendees can leave with practical approaches and strategies for data exploration.
* Stoke Curiosity: Help participants see data exploration as an exciting step and shift attitudes from accepting data at face value to actively questioning and probing data to uncover underlying issues, patterns, anomalies, and trends.

## Setup Documentation
### Folder and Files
INPUTS: Input data of watershed characteristics is not included in this repository. Download the data from [FigShare repository](https://figshare.com/s/da62fabe5e2ba6cdc6a0). Contents of the INPUTS folder are:
- **workshop_DataExploration.yml**: virtual environment .yml file. See notes below for import. 
- **WtshdAttributeTable_20240603.txt**: Watershed attribute data file.
- **CQ_Data_20240604.txt**: Paired concentration and discharge recording for 2594 watersheds from 1980 to 2020.
- **Dataset_XX**: Raw watershed attributes input folders each contain a textfile with watershed characteristics. 
- **boundaries-shapefiles-by-aggeco/**: Folder that contains watershed shapefile.
- **cb_2017_us_state_5m/**: Folder that contains US state boundary.

CODE: Jupyter notebooks created for downloading data and processing data.
- **DATA_datasetCompilation.ipynb** compiles watershed attributes and downloading water flow and concentration data. The output of this script is 'WtshdAttributeTable_20240603.txt' and 'CQ_Data_20240604.txt'.
- **ANA_dataExploration.ipynb** performs the analysis and data exploration of the watershed's concentration-discharge and attribute analysis. 

### Software
You are free to use any software/online platform you prefer for the workshop. If you are new to Python, I recommend starting with Anaconda, which simplifies package management and deployment.

To setup the environment through conda, install conda (Anaconda or miniconda). 
Once downloaded, you can create your environment by importing the config _YAML_ I have provided. This contains all the packages you will need to install for the workshop. 
1. Open the Anaconda Prompt (or your terminal if using Miniconda).
2. Navigate to the directory containing the configuration _YAML_ file (e.g., INPUTS/). You can use the cd command to change directories. 
`cd path/to/your/INPUTS/`
3. Run the following commands:
```
conda env create -f workshop_DataExploration.yml
conda activate workshop_DataExploration
```
- The first command creates a new environment based on the specifications in the workshop_DataExploration.yml file.
- The second command activates the newly created environment.
4. Next download Jupyter Notebook and run it
```
conda install jupyter
jupyter notebook
```
5. Register your kernel
```
conda activate workshop_DataExploration 
conda install ipykernel python -m ipykernel install --user --name workshop_DataExploration
python -m ipykernel install --user --name workshop_DataExploration
``

This workshop is accessible through [my Github](https://github.com/danykakbyrnes/DataExplorationWorkshop.git).