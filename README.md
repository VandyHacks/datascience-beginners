# How to do Data Science in 10 minutes of Python
*For the hackers at VandyHacks 2018*

# Preface 
This guide is to help you get set up with a popular environment for data science in Python and to introduce some next steps.

Doing data science is a little different than traditional dev work because it is meant to be **interactive** and **deliberate**. Working on a visual environment like Jupyter Notebooks will really help you do the most with your data. Notebooks consist of cells which can show Markdown or Python. This lets you execute code incrementally, as opposed to running an Python file from start-to-finish. This is very useful for making small changes and making progress. 

### Helpful Links 
Use these if you don't like this guide

1. A full guide to Jupyter installation and usage: http://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/what_is_jupyter.html

2. A more detailed version of this guide (with pictures!): https://www.dataquest.io/blog/jupyter-notebook-tutorial/

# Part 1. Your Environment 

Setting up your environment is one of the harder steps in starting data science with Python. The holy trifecta of Python data-processing modules consists of `pandas`, `numpy`, and `matplotlib`. Jupyter Notebooks are likely the best 'IDE' in the field. After these are installed, "data science" is mostly about Googling `pandas` and `matplotlib` syntax.

## A. The easiest way
If you want to get started immediately, you can just head over to [Microsoft Azure Notebooks](https://notebooks.azure.com). This is actually a pretty good service and hosts Jupyter Notebook servers for you. 
1. **Sign In** on the top-left with a Microsoft account. (You can also hit "Get Started" on the main page to look at some samples.)
2. Hit **Libraries** on the header and make a new library. A library is just a folder on this platform.
3. In a library, hit **New**. You want **Item Type** to be *Python 3.6 Notebook* or whichever Python version you prefer. Give the notebook a name like **test.ipynb** and create it.
4. Click on the new notebook in your library. Within a minute, you should have a Jupyter Notebook up and running. 

## B. The traditional way (skip if you took method A)
Note that a locally installed environment is faster than the Azure Notebooks, but they are not painfully slow and should be enough. However, if you want more customization with the Jupyter runtime or just want this on your local machine, you can follow the steps below. 

(If you are experienced, just install Jupyter and all aforementioned needed Python modules with `pip`.)

1. **Install Anaconda**: https://www.anaconda.com/download/ 
	Note: this also installs Python if you don't have it
2. **Install Jupyter**: 
	Open a terminal. Try if typing `jupyter notebook` says something other than 'command not found'. If not, you [may need to set your environment variables](https://stackoverflow.com/questions/44597662/conda-command-is-not-recognized-on-windows-10).

3. **Run a notebook**:
	Open a browser and go to `localhost:8888` (or whichever port the console says) 
	You can make a new notebook by going to the top right **New** -> **Python 3**

## More options
Look for guides on setting up Jupyter on a GCP Compute Engine or AWS EC2 if you need *a lot* of computing resources. Also, look into GCP BigQuery if your data is quite large for a single machine (10s of gigabytes). 

# Part 1a. Using a notebook 
- A notebook is made of **cells**. Run a cell with `Ctrl + Enter`. 

Jupyter has 2 main modes: *Command* and *Edit*. 
- When you press `Enter` on a cell, you can *edit* it. 
- `esc` brings you into command mode. Here, add cells with `b` and delete cells by hitting `d` twice. Move with arrow keys. 
- The top toolbar lets you see all Keyboard Shortcuts, and the keyboard icon button lets you search for a command.
- Play around to explore more features (like Markdown cells)

- **Remember to save your notebooks before shutting down the server!** You can see if your notebook is saved in the console running Jupyter. `Ctrl + C` to close Jupyter. 

# Part 2. Data 
This section refers to another Notebook showcasing how some basic data handling is done. 

Please follow along the notebook in this repo [**Tutorial.ipynb**](https://github.com/VandyHacks/datascience-beginners/blob/master/Tutorial.ipynb).

For an interactive version, use our [Azure Notebooks library](https://notebooks.azure.com/kennli/libraries/vh-datascience-beginners) and click on **Tutorial.ipynb**.

### Helpful Links 

1. 10 Minutes to pandas - https://pandas.pydata.org/pandas-docs/stable/10min.html 
2. Kaggle datasets (Lots of clean data on many topics) - https://www.kaggle.com/datasets
3. AI/ML services:
	a. Azure ML Studio - https://studio.azureml.net/
	b. IBM Watson - https://www.ibm.com/watson/developer/
4. Pandas cheatsheet - https://github.com/pandas-dev/pandas/blob/master/doc/cheatsheet/Pandas_Cheat_Sheet.pdf 


The main steps to actually doing something on Jupyter look something like this:

1. **Load your data and process it**. Start with importing your packages and making sure you can see your data. If importing a package yields an error (ex. "package not found"), open up another terminal and install it with `pip` or `conda`. 

2. **Make some graphs**. Matplotlib is a full visualization suite and can be complemented with `seaborns`. Feel free to use `plt.plot`, `plt.hist`, `plt.bar`, etc. 

3. **Get some insights**. Think of 2-3 nontrivial questions you want answers. Work out the steps needed to be taken and extract answers from your data. Usually this will involve a lot of filtering, cleaning, plots, etc. In this stage, StackExchange and Google are your main consultants. 

