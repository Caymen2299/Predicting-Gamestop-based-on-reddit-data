# Predicting-Gamestop-based-on-reddit-data
Fully connected Neural Network filled with dense layers that tries to show correlation between reddit data and gamestop stock by by trying to predict closing prices

# Instructions on how to install software used in project:
### Conda installed?
    Yes: move on to step 2
    No: go to https://www.anaconda.com/products/individual and download and install the conda version right for your operating system
### Python installed?
    Yes: move to step 3
    No: download latest version of python here: https://www.python.org/downloads/ 
### Create a new conda environment in a terminal by tying the command: conda create --name_of_env_here python=python_version_here
    Example: conda create --capstone python=3.7
### Activate your environment by running the command below
    conda activate name_of_env
### Install libraries used with commands below
    pip install -U scikit-learn
    pip install tensorflow
    conda install numpy
    conda install pandas
    conda install -c anaconda pandas-datareader
    conda install matplotlib
    pip install jupyter
    pip install requests
    pip install datetime3
### Open jupyter notebook by typing in the terminal: jupyter-notebook

## Running the dataset maker
### Important! This part is optional and should only be run if a user wants to create a new dataset. The dataset used in training is included in the project files. This pulls down posts from reddit and pulls down closing prices from yahoo into separate csv files. The combination of these two datasets was done in excel to create the final dataset otherwise known as the WSB dataset or WSBdataAndClosingInfo.csv 
Navigate to the folder containing the project and then open the makeDataset.ipynb file. 
Follow directions on https://towardsdatascience.com/how-to-use-the-reddit-api-in-python-5e05ddfd1e5c on how to set up a bot on reddit (step 1 through 3)
Enter Client ID into the first cell where it says “client_id_here”
Enter Client Secret into the first cell where it says “client_secret_here”
Enter your username and password into the data dictionary named data_dict
Run the program. 
Format the dataset in excel to match dates and pricing for posts.

## Running the neural network
Navigate to the folder containing the project and then navigate to  predicting_gamestop_nn.ipynb file. 
Open the file and run the entire program
Make sure to give the program time as it takes a while to run due to the training.
