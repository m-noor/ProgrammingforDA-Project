# Programming for Data Analysis - Project
## Project for the GMIT HDip in Data Analysis Course

### Brief introduction
This repository is concerned with the use of Python `numpy.random` and `scipy.stats` packages as well as a statistical technique (inverse transform sampling) to generate a synthetic dataset. For this purpose, the CASP dataset is used. This repository contains the following files:

1. [README.md](README.md) (this file)
1. [ProgrammingforDA-Assignment.ipynb](ProgrammingforDA-Assignment.ipynb) - a Jupyter Notebook written in Python
1. [ProgrammingforDA-Assignment.pdf](ProgrammingforDA-Assignment.pdf) - PDF version of the Notebook. Note this is for reference only as the notebook is not accurately reproducible through conversion to PDF.
1. [ProgrammingforDA-Assignment.html](ProgrammingforDA-Assignment.html) - HTML version of the Notebook. Note this is for reference only as the notebook is not accurately reproducible through conversion to HTML, although some interactivity is still retained as Plotly uses JavaScript natively.
1. [Programmingfor-DA-assignment-instructions.pdf](Programmingfor-DA-assignment-instructions.pdf) - instructions for the assignment, for future reference only

* Note that GitHub places a limit of 25 MB for file upload via web browser and 100 MB for GitHub Desktop and git. As the size of this notebook is quite large (especially some of the commits), the Jupyter Notebook is stored on Git Large File Storage (LFS).*

### Pre-requisites for running the notebook
This notebook relies on the following libraries, so please ensure you have these installed on your machine before running.

1. `numpy`
1. `plotly`
1. `scipy`
1. `orca` to generate static Plotly plots - see reference

### Troubleshooting / known issues
By default, Plotly plots are fully interactive and editable with the free tool, Chart Studio. However, as each plot actually contains the data points within itself, rather than referencing variables, the notebook size can be quite large especially for a large dataset such as the CASP. Due to this, interactivity in plots is sacrified for notebook size by converting all the plots into images inline. In other words, these images are not saved locally but are generated within the Python memory space and displayed after conversion as images within the Jupyter notebook cells.
