[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kaust-vislab/W2I-machine-learning-bootcamp/master?urlpath=lab)
[![GitPitch](https://gitpitch.com/assets/badge.svg)](https://gitpitch.com/kaust-vislab/W2I-machine-learning-bootcamp/master?grs=github)

# W2I-machine-learning-bootcamp

* Day 1 of the workshop will largely follow the Software and Data Carpentry's [Plotting and Programming in Python](http://swcarpentry.github.io/python-novice-gapminder/) lecture. Additional material may be drawn from the lesson on [Programming in Python](http://swcarpentry.github.io/python-novice-inflammation/) as needed. 

* Day 2 of the workshop will cover any remaining material from the Software Carpentry lectures before moving on to cover chapter two of [_Hands-on Machine Learning with Scikit-learn and TensorFlow._](https://proquest.safaribooksonline.com/9781491962282)

Days 3-5 will cover in more detail various approaches from classical machine learning and deep learning.

# Installation instructions

## 0. Install Git

### Linux or Mac OS
Install the latest version of [Git](https://git-scm.com/downloads) version control system for your operating system.

### Windows
Download instructions for Windows are a bit more involved.

1. Download the [Git for Windows](https://gitforwindows.org/) installer.
2. Run the installer and follow the steps below:
    * Click on "Next" four times (two times if you've previously installed Git). You don't need to change anything in the information, location, components, and start menu screens.
    * Select “Use the nano editor by default” and click on “Next”.
    * Keep "Use Git from the Windows Command Prompt" selected and click on "Next". If you forgot to do this programs that you need for the workshop will not work properly. If this happens rerun the installer and select the appropriate option.
    * Click on "Next".
    * Keep "Checkout Windows-style, commit Unix-style line endings" selected and click on "Next".
    * Select "Use Windows' default console window" and click on "Next".
    * Click on "Install".
    * Click on "Finish".
3. If your "HOME" environment variable is not set (or you don't know what this is):
    * Open command prompt (Open Start Menu then type cmd and press [Enter])
    * Type the following line into the command prompt window exactly as shown: `setx HOME "%USERPROFILE%"`
    * Press [Enter], you should see `SUCCESS: Specified value was saved.`
    * Quit command prompt by typing exit then pressing [Enter]

## 1. Install Anaconda
Install the Python 3.7 version of either [Anaconda](https://www.anaconda.com/distribution/) or [miniconda](https://docs.conda.io/en/latest/miniconda.html). 

## 2. Clone the workshop repository using Git
Open a terminal window (Linux or Mac OS). On Mac OS the terminal can be found in`/Applications/Utilities/` folder (I recommend adding the terminal to your dock!). On Windows open a Git Bash Shell (shortcut should be on your desktop!). Now type the following command at the prompt to clone the workshop repository.

```bash
$ git clone https://github.com/kaust-vislab/W2I-machine-learning-bootcamp.git
```
There is another repository of notebooks that you will need for day 5 which you might as well go ahead and clone now.

```bash
$ git clone https://github.com/bentrevett/pytorch-sentiment-analysis.git
```

## 3. Create the Conda environment 
From your terminal, change into the workshop directory and run the following command to create the conda environment.

```bash
$ cd W2I-machine-learning-bootcamp/
$ conda env create -f environment.yml
```

## 4. Activate the Conda environment
From your terminal, run the following command to activate the conda environment.

```bash
$ source activate W2I-machine-learning-bootcamp
```

## 5. Start JupyterLab
Once the environment is active you can run the following command to start JupyterLab.
```
$ jupyter lab
```

## Additional Resources

### Core Data Science tools

In addition to knowledge of Python an aspiring data scientist you should seek to develop proficiency in the following areas:

* Version control using [Git](https://git-scm.com/) and either [GitHub](https://github.com/) or [GitLab](https://about.gitlab.com/).
* SQL programming for extracting data from relational databases.
* The Unix shell for interacting with clusters in the cloud ([GCP](https://cloud.google.com/), [AWS](https://aws.amazon.com/), [Azure](https://azure.microsoft.com/en-us/), etc)
* Container-based work flows using [Docker](https://www.docker.com/) to enable your data science pipelines to run on your laptop, on cluster, even on HPC (without changing your code!).

In addition to the Python lessons that we will cover in the workshop, [The Carpentries](https://carpentries.org) have excellent introductory materials on [version control using Git](http://swcarpentry.github.io/git-novice), [Bash Shell]([http://swcarpentry.github.io/shell-novice) and [SQL](http://swcarpentry.github.io/sql-novice-survey) as well as a number of more [domain-specific data-science lessons](https://datacarpentry.org/lessons/) that are built on this tool stack. There is also a lesson on [Testing and Continuous Integration with Python](http://katyhuff.github.io/python-testing/) which covers how to build automated testing infrastructure for you research software and data analysis.

#### Jupyter Notebooks

Here are a few Jupyter notebook cheat sheets that I have encountered and found useful.

* [Anaconda Jupyter Notebook Cheatsheet](https://docs.anaconda.com/_downloads/JupyterLab-Notebook-Cheatsheet.pdf)
* [DataCamp Jupyter Notebook Cheatsheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Jupyter_Notebook_Cheat_Sheet.pdf])

### Machine Learning and Deep Learning

The following is a non-exhaustive list of Python for data science books and courses that I have found useful in my career as a data scientist.  **If you have a good learning resource that is not listed here please share!**

#### Books

There are a number of excellent books available all of which have source code (i.e., Jupyter notebooks) available for download via GitHub. 

* [Python for Data Analysis, 2nd Edition](http://shop.oreilly.com/product/0636920050896.do) ([source code](https://github.com/wesm/pydata-book)) 
* [Python Data Science Handbook](http://shop.oreilly.com/product/0636920034919.do) ([source code](https://github.com/jakevdp/PythonDataScienceHandbook))
* [Hands-on Machine Learning with Scikit-Learn and Tensorflow](http://shop.oreilly.com/product/0636920052289.do)([source code](https://github.com/ageron/handson-ml))
* [Deep Learning with Python](https://www.manning.com/books/deep-learning-with-python) ([source code](https://github.com/fchollet/deep-learning-with-python-notebooks))
* [Tensorflow for Deep Learning](http://shop.oreilly.com/product/0636920065869.do) ([source code](https://github.com/matroid/dlwithtf))

#### Courses

Python-based on-line data science training courses to dig deeper into a particular topic.

##### Udacity Nanodegree programs

* [AI Programming with Python](https://sa.udacity.com/course/ai-programming-python-nanodegree--nd089)
* [Become a Data Scientist](https://sa.udacity.com/course/data-scientist-nanodegree--nd025)
* [Become a Machine Learning Engineer](https://sa.udacity.com/course/machine-learning-engineer-nanodegree--nd009)
* [Deep Learning](https://sa.udacity.com/course/deep-learning-nanodegree-foundation--nd101)
* [Natural Language Processing](https://sa.udacity.com/course/natural-language-processing-nanodegree--nd892)
* [Deep Reinforcement Learning](https://sa.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893)

##### Coursera Specializations

* [Applied Data Science with Python](https://www.coursera.org/specializations/data-science-python)
* [Deep Learning](https://www.coursera.org/specializations/deep-learning)
* [Machine Learning with TensorFlow on Google Cloud Platform](https://www.coursera.org/specializations/machine-learning-tensorflow-gcp)
* [Advanced Machine Learning with TensorFlow on Google Cloud Platform](https://www.coursera.org/specializations/advanced-machine-learning-tensorflow-gcp)
* [Data Engineering on Google Cloud Platform](https://www.coursera.org/specializations/gcp-data-machine-learning)
* [Advanced Machine Learning](https://www.coursera.org/specializations/aml)
* [Genomic Data Science](https://www.coursera.org/specializations/genomic-data-science)

##### Others

* Various Deep and Machine Learning Courses from [fast.ai](https://www.fast.ai/).

