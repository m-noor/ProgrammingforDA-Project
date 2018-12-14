# Programming for Data Analysis - Project
## Project for the GMIT HDip in Data Analysis Course

### Brief introduction
This repository is concerned with the use of Python `numpy.random` and `scipy.stats` packages as well as a statistical technique (inverse transform sampling) to generate a synthetic dataset. For this purpose, the [CASP dataset](http://archive.ics.uci.edu/ml/datasets/Physicochemical+Properties+of+Protein+Tertiary+Structure) is used. This repository contains the following files:

1. [README.md](README.md) (this file)
1. [CASP.csv](CASP.csv) - input dataset
1. [CASP_synthetic_inverse_transform_sampling.csv](CASP_synthetic_inverse_transform_sampling.csv) - output file of synthetic values generated using the inverse transform sampling method
1. [CASP_synthetic_standard_distributions.csv](CASP_synthetic_standard_distributions.csv) - output file of synthetic values using standard (well-known) probability distributions
1. [ProgrammingforDA-Project.html](ProgrammingforDA-Project.html) - HTML version of the Jupyter notebook. Note this is for reference only as the notebook is not accurately reproducible through conversion to HTML.
1. [ProgrammingforDA-Project.ipynb](ProgrammingforDA-Project.ipynb) - a Jupyter notebook written in Python 3.6*
1. [ProgrammingforDA-Project.pdf](ProgrammingforDA-Project.pdf) - PDF version of the Jupyter notebook. Note this is for reference only as the notebook is not accurately reproducible through conversion to PDF.
1. [distribution_chart.gif](distribution_chart.gif) - an image for illustration purpose referenced within the Jupyter notebook
1. [overfit_underfit.png](overfit_underfit.png) - an image for illustration purpose referenced within the Jupyter notebook
1. [ProgrammingforDA-project-instructions.pdf](ProgrammingforDA-project-instructions.pdf) - instructions for the project, for future reference only.


* *Note that GitHub places a limit of 25 MB for file upload via web browser and 100 MB for GitHub Desktop and git. As the size of this notebook is quite large (especially some of the commits), the Jupyter Notebook is actually stored on [Git Large File Storage (LFS)](https://git-lfs.github.com/). Please read [this page](https://help.github.com/articles/collaboration-with-git-large-file-storage/) before cloning and pushing to this repository.*

### Pre-requisites for running the notebook
This notebook relies on the following libraries, so please ensure you have these installed on your machine before running.

1. `numpy`
1. `plotly`
1. `scipy`
1. `orca` to generate static Plotly plots - see reference
1. `fitter`- the original fitter is available [here](https://pypi.org/project/fitter/). However, as the last commit was about 2 years ago, and with the updates to `matplotlib` since then, a [forked `fitter` will be used](https://github.com/caiostringari/fitter/tree/master). To install, use the command prompt/shell and execute the following: `pip install --upgrade https://github.com/caiostringari/fitter/tarball/master`. The `--upgrade` option can be omitted if there is no pre-existing `fitter` library.

### Troubleshooting / known issues
By default, Plotly plots are fully interactive and editable with the free tool, Chart Studio. However, as each plot actually contains the data points within itself, rather than referencing variables, the notebook size can be quite large especially for a large dataset such as the CASP. Due to this, interactivity in plots is sacrified for notebook size by converting all the plots into images inline. In other words, these images are not saved locally but are generated within the Python memory space and displayed after conversion as images within the Jupyter notebook cells.
