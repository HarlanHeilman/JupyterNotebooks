# Intro to Jupyter
### *Harlan Heilman*

Notebook documents or notebooks are documents produced by the Jupyter Notebook App, which contain both computer code (e.g. python) and rich text elements (paragraph, equations, figures, links, markdown, etc…). Notebook documents are both human-readable documents containing the analysis description and the results (figures, tables, etc..) as well as executable documents which can be run to perform data analysis.

There are several apps that are used to run notebooks but the most common two are Jupyter Lab for a more modern browser gui, and the classica Jupyter notebook. To install these, I recomend first installing [Anaconda](https://www.anaconda.com/) on your personal computer and then using it to install [Jupyter lab/notebook](https://docs.anaconda.com/navigator/overview/#navigator-pages). Alternately, this can be ran using a remote server and acessed theough the internet. 

## Packages to install
Once Anaconda and Jupyter are installed use the start menue to open an anaconda terminal as administrator. Once it is opened we will want to install the following packages. These usually come with Anaconda, but just to be sure copy and paste the following command into the anaconda terminal and run. 

`conda install numpy matplotlib scipy sys pandas`

This installs the needed packages to go though the included Jupyter notebooks.

We will also need to install a package for dealing with the .edf files. The best package I found for this is [FabIO](https://pythonhosted.org/fabio/install.html) and it requires the following install. 

`conda install setuptools wheel fabio`

This will allow us to get both header information and data from the binary .edf file.
