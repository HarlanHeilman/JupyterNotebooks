# Intro to Jupyter
### *Harlan Heilman*

Notebook documents or notebooks are documents produced by the Jupyter Notebook App, which contain both code (e.g. python) and rich text elements (paragraph, equations, figures, links, markdown, etc…). Notebook documents are both human-readable documents containing the analysis description and the results (figures, tables, etc..) as well as executable documents which can be run to perform data analysis.

There are several apps that are used to run notebooks but the most common two are Jupyter Lab for a more modern gui, and the classical Jupyter notebook witch is more bare bones. Luckily, both of these apps come with [Anaconda](https://www.anaconda.com/), a one stop shop for most things python and data science. 

## Installing Anaconda

To install Anaconda, navigate to the web page [Anaconda](https://www.anaconda.com/) and select to download now. Open the downloaded executable and follow the recomended download instructions. 

- [ ] Once we are done instaling Anaconda, navigate to Anaconda Navigator(Anaconda3) and run the program as an admin (This is needed to install packages). Ensure that you are in the base (root) enviroment before proceeding. 
- [ ] Launch the CMD.exe Prompt to open a terminal in the (base) enviroment. 

## Quick Install method

To install the required packages for the notebooks in theis repo, copy and paste the folloiwing line into the terminal and hit enter to run. 

```
conda install numpy matplotlib scipy sys pandas setuptools wheel uncertainties
```


This installs the `numpy`, `matplotlib`, `scipy`, `sys`, `pandas`, `setuptools`, `wheel`, and `fabio` python packages. This gives you acess to any functions in the packages and allows you to include these functions into any scripts in your (base) enviroment. 

## Recomended Install Method

It is recomended to build an enviroment that you can use in the future for all your xray data analysis. We do this in anaconda, we first create a new enviroment:

```
conda create -n xray python=3.7 numpy scipy pandas matplotlib
```

Enter the new enviroment and finish installing packages as needed, copy the lines that dont start with (#)

```
# Activate environment
activate pypxr

# Install Required Packages
conda install uncertainties setuptools wheel fabio 
```

