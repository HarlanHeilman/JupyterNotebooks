# Intro to Jupyter
### *Harlan Heilman*

Notebook documents or notebooks are documents produced by the Jupyter Notebook App, which contain both code (e.g. python) and rich text elements (paragraph, equations, figures, links, markdown, etc…). Notebook documents are both human-readable documents containing the analysis description and the results (figures, tables, etc..) as well as executable documents which can be run to perform data analysis.

There are several apps that are used to run notebooks but the most common two are Jupyter Lab for a more modern gui, and the classical Jupyter notebook witch is more bare bones. Luckily, both of these apps come with [Anaconda](https://www.anaconda.com/), a one stop shop for most things python and data science. 

## Installing Anaconda

To install Anaconda, navigate to the web page [Anaconda](https://www.anaconda.com/) and select to download now. Open the downloaded executable and follow the recomended download instructions. 

- [ ] Once we are done instaling Anaconda, navigate to Anaconda Navigator(Anaconda3) and run the program as an admin (This is needed to install packages).

![image](https://user-images.githubusercontent.com/73567020/211663849-6152969b-fb96-4ceb-8772-34b0d071edf6.png)

Ensure that you are in the base (root) enviroment before proceeding. 

![image](https://user-images.githubusercontent.com/73567020/211663919-e30e9ce7-b26d-421b-9a8f-beb7cb65a61a.png)

- [ ] Launch the Powershell Prompt Prompt to open a terminal in the (base) enviroment. 

![image](https://user-images.githubusercontent.com/73567020/211677774-e826bd70-d8fd-4402-afc1-6027840f583b.png)

## Quick Install method

To install the required packages for the notebooks in theis repo, copy and paste the folloiwing line into the terminal and hit enter to run. 

```
conda install numpy matplotlib scipy pandas setuptools wheel uncertainties
```


This installs the `numpy`, `matplotlib`, `scipy`, `pandas`, `setuptools`, `wheel`, and `fabio` python packages. This gives you acess to any functions in the packages and allows you to include these functions into any scripts in your (base) enviroment. 

## Recomended Install Method

It is recomended to build an enviroment that you can use in the future for all your xray data analysis. We do this in anaconda, we first create a new enviroment:

```
conda create -n xray python=3.7 numpy scipy pandas matplotlib
```

To enter this new xray enviroment and finish installing packages as needed, copy the lines that dont start with (#)

```
# Activate environment
conda activate xray

# Install Jupyterlab in the new xray enviroment
pip install jupyterlab ipywidgets

# Useful  Packages to include
pip install uncertainties setuptools wheel fabio 
```

Once this is done feel free to close your terminal and swap to your new xray eviroment. 

![image](https://user-images.githubusercontent.com/73567020/211678728-cabea0f1-35af-4132-936f-82dede5d8044.png)


## Opening A Notebook

Once everything above is compleated, start by [downloading this repo](https://www.itpro.com/software/development/359246/how-to-download-from-github) and you will be able to acess any of the files for your own purposes. Once the repo is installed. Using the Anaconda Navigator, launch JupyterLab. This will open a notebook editor IDE in your default browser. With this open, you will see a side panel that gives you your working directory. 

![image](https://user-images.githubusercontent.com/73567020/211663735-c2e4549a-fa8f-4cb1-8f47-7071e1c22de2.png)

From here you will want to navigate to the install location of your github repository. When finished you should see something like this 

![image](https://user-images.githubusercontent.com/73567020/211663690-4512e16e-a8a9-4000-a36f-48eb2191be9e.png)

From here we can click to open any files you want I recomend starting with **curvefit1.ipynb** or **Fitting.ipynb**. Please reach out with any questions 

