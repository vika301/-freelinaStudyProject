# FreelinaStudyProject

For a study project at the TU Chemnitz in Germany twitterdata of several weeks has been collected without academic or developer access via the twitterexplorer (https://github.com/pournaki/twitter-explorer). These jupyter notebooks were used to concatenate the seperatley pulled datasets(CleaningFiles.ipynb), which only can capture data from 7 days each and to clean them from duplicates(ConcatenadeFiles.ipynb). In the following an instruction for the process of datacollection and requirements is provided, followed by an instrution to recreate the Hashtagnetwork with the provided cleaned dataset 'Cleaned.csv'.

# Recreate the Process:
1. Install Anaconda or Miniconda (https://docs.anaconda.com/anaconda/install/index.html)
2. Install Jupyter Notebook / Lab in the base environment (https://jupyter.org/install)
3. Install a new environment
```sh
conda create --name twit
```
4. Activate the environment for Jupyter Notebook
```sh
conda activate --name twit
```
5. Install the twitterexplorer-Software with the provided instructions(https://github.com/pournaki/twitter-explorer).
6. Get all requirements 
```sh
pip install -r requirements.txt
```

# Recreate the Hashtagnetwork with the preinstalled twitterexplorer:

7. Unzip the 'datafreelina'-folder in the current directory and first run the CleaningFiles.ipynb and after the ConcatenadeFiles.ipynb
8. Run the visualizer.py of the twitterexplorer with the generated dataset 'Cleaned.csv'.
9. Specify the date from 28. 05.2022 - 18.07.2022, set the hashtag- and edge-reduction to 0 in order to view the whole dataset and activate the Leiden-Community detection algorithm. The html-file with the generated network can now be found in the outputfolder of the twitterexplorer-folder.

# Acknowledgement
Pournaki, A., Gaisbauer, F., Banisch, S., & Olbrich, E. (2021). The Twitter Explorer: A Framework for Observing Twitter through Interactive Networks. Journal of Digital Social Research, 3(1), 106–118. https://doi.org/10.33621/jdsr.v3i1.64
