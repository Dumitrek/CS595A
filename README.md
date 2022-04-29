# CS595A Final Project
This repository is the accumulated work of the CS595A Final Project conducted by Kevin Dumitrescu, Victoria Jordan, and Ozgur Ural. The goal of the project is to be able to take a User Generated Spotify Playlist and a Spotify Generated Recommended Playlist and compare the Audio Features between the two playlists using a series of Regression algorithms to determine how accurate is Spotify's Recommendation system in terms of generating new playlists within close relation a user created playlist. In terms of how we were able to collect the Audio Features for each constructed playlist, we utilized the Spotipy library to be able to authenticate that we were the user trying to access our own playlists, and then pull the track data relevant of both the User and Recommneded playlist into their own respective Pandas dataframes and then downloaded into their own respective JSON files.

# 1. Project Installation

In order to install the project, you must first have an environment in which you can operate Jupyter Notebooks.

In the case that you have already have set up an environment, then proceed with downloading the Jupyter Notebooks listed below. 

### 1.1 Installing the Jupyter Notebooks

For the *UserExtract* and the *RecommendedExtract_1* Jupyter notebooks, this can be achieved through selecting the *Raw* button on the file. This will pull up a new window showcasing the code to which you can then press *CTRL+S* on your keyboard to then pull up the file explorer to then save each file. Do note that this will default save as a *.txt* file and thus in order to properly format this back into a Jupyter notebook, remove the *.txt* when you upload the files into your Jupyter Notebook environment. This can be done by first opening the file within your Jupyter Notebook environment, selecting on the file name at the top of the newly opened file, and lastly removing the previously aforementioned *.txt* file extension. Once removed, close the file and this shall then automatically revert the files into Jupyter Notebooks.

For the Regression Jupyter Notebook, this can be achieved through selecting the *Download* button on the file. This will pull up a new window showcasing the code to which you can then press *CTRL+S* on your keyboard to then pull up the file explorer to then save each file. Do note that this will default save as a *.txt* file and thus in order to properly format this back into a Jupyter notebook, remove the *.txt* when you upload the files into your Jupyter Notebook environment. This can be done by first opening the file within your Jupyter Notebook environment, selecting on the file name at the top of the newly opened file, and lastly removing the previously aforementioned *.txt* file extension. Once removed, close the file and this shall then automatically revert the files into Jupyter Notebooks.

[AI_Final_Project_Dumitrescu_Jordan_Ural_v5.0_-_UserExtract.ipynb](https://github.com/Dumitrek/CS595A_Final_Project/blob/main/Jupyter%20Notebook%20Code/AI_Final_Project_Dumitrescu_Jordan_Ural_v5.0_-_UserExtract.ipynb)

[AI_Final_Project_Dumitrescu_Jordan_Ural_v5.0_-_RecommendedExtract_1.ipynb](https://github.com/Dumitrek/CS595A_Final_Project/blob/main/Jupyter%20Notebook%20Code/AI_Final_Project_Dumitrescu_Jordan_Ural_v5.0_-_RecommendedExtract_1.ipynb)

[AI_Final_Project_Dumitrescu_Jordan_Ural_v5.0_Regression.ipynb](https://github.com/Dumitrek/CS595A_Final_Project/blob/main/Jupyter%20Notebook%20Code/AI_Final_Project_Dumitrescu_Jordan_Ural_v5.0_Regression.ipynb)

### 1.2 Installing the JSON files

In the event that you do not wish to generate your own JSON files for testing purposes, simply download the JSON fles provided below. After downloading them onto your PC, simply upload them into the same environment to which the previous three Jupyter Notebooks reside. Failure to include them within the same space will cause the Regression Jupyter Notebook to not function and will generate errors based on the missing JSON files.

[user_json.json](https://github.com/Dumitrek/CS595A_Final_Project/blob/main/JSON%20Data%20Files/user_json.json)

[rec_json.json](https://github.com/Dumitrek/CS595A_Final_Project/blob/main/JSON%20Data%20Files/rec_json.json)


# 2. Project Execution

Once all files have been installed within your Jupyter Notebook enviroment, open the three Jupyter Notebooks. At the top of each notebook is a labeled number of 1, 2, and 3. This numbers indicate the ordering to which the Notebooks need to be executed.

*If you have downloaded the "user_json.json" and the "rec_json.json" files provided and they are in the same space as the Regression notebook, then skip to section 2.3 titled Running Regression Notebook.

### 2.1 Running UserExtract Notebook

If you have note downloaded the *user_json.json* file, you can then execute this code. Simply start from the beginning by selecting the first cell and then procedurally run each cell till you have executed the final cell within the Notebook. Once the final cell has been executed, the *user_json.json* file will be generated within your *Downloads* folder on your PC. From there simply follow the instructions provided in section 1.2 to install your generated file into your Jupyter Notebook Environment.

### 2.2 Running RecommendedExtract Notebook

If you have note downloaded the *rec_json.json* file, you can then execute this code. Simply start from the beginning by selecting the first cell and then procedurally run each cell till you have executed the final cell within the Notebook. Once the final cell has been executed, the *rec_json.json* file will be generated within your *Downloads* folder on your PC. From there simply follow the instructions provided in section 1.2 to install your generated file into your Jupyter Notebook Environment.

### 2.3 Running Regression Notebook 

Once the *user_json.json* and the *rec_json.json* files have been installed into the same space as the *Regression* notebook, simply start from the beginning by selecting the first cell and then procedurally run each cell till you have executed the final cell within the Notebook. Some cells, like the generation of the *ScatterPlot Matrix* will take longer in execution time to output. Once the final cell has been executed, the results of each Regression algorithm utilized to test each Audio Feature of the Spotify Recommended Playlist to the User Generated Playlist shall be displayed in a means of scoring accuracy.
