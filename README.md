[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kaust-vislab/W2I-machine-learning-bootcamp/master?urlpath=lab)
[![GitPitch](https://gitpitch.com/assets/badge.svg)](https://gitpitch.com/kaust-vislab/W2I-machine-learning-bootcamp/master?grs=github)

# W2I-machine-learning-bootcamp

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
* The Unix shell for interacting with clusters either locally at KAUST (i.e., Ibex, Nesser, Shaheen, etc) or in the cloud ([[https://cloud.google.com/ | GCP]], [[https://aws.amazon.com/ | AWS]], [[https://azure.microsoft.com/en-us/ | Azure]], etc)
* Container-based work flows using [[https://www.docker.com/ | Docker]] to enable your data science pipelines to run on your laptop, on cluster, even on HPC (without changing your code!).

In addition to the Python lessons that we will cover in the workshop, [[https://carpentries.org/ | The Carpentries]] have excellent introductory materials on [[http://swcarpentry.github.io/git-novice | version control using Git]], [[http://swcarpentry.github.io/shell-novice | Unix shell commands]], [[http://swcarpentry.github.io/r-novice-gapminder/ | R]], and [[http://swcarpentry.github.io/sql-novice-survey/ | SQL]] as well as a number of more [[https://datacarpentry.org/lessons/ | domain-specific data science lessons]] that are built on this tool stack. There is also a lesson on [[http://katyhuff.github.io/python-testing/|Testing and Continuous Integration with Python]] which covers how to build automated testing infrastructure for you research software and data analysis.

#### Jupyter Notebooks

Here are a few Jupyter notebook cheat sheets that I have encountered and found useful.

* [[https://docs.anaconda.com/_downloads/JupyterLab-Notebook-Cheatsheet.pdf | Anaconda Jupyter Notebook Cheatsheet]]
* [[https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Jupyter_Notebook_Cheat_Sheet.pdf | DataCamp Jupyter Notebook Cheatsheet]]

### Machine Learning and Deep Learning

The following is a non-exhaustive list of Python for data science books and courses that I have found useful in my career as a data scientist.  **If you have a good learning resource that is not listed here please share!**

#### Books

There are a number of excellent books available all of which have source code (i.e., Jupyter notebooks) available for download via GitHub. 

* [Python for Data Analysis, 2nd Edition](http://shop.oreilly.com/product/0636920050896.do) ([[https://proquest.safaribooksonline.com/9781491957653 | Full Text Online]]) ([[https://github.com/wesm/pydata-book | source code]]) 
* [[http://shop.oreilly.com/product/0636920034919.do | Python Data Science Handbook]] ([[https://proquest.safaribooksonline.com/9781491912126 | Full Text Online]]) ([[https://github.com/jakevdp/PythonDataScienceHandbook | source code]])
* [[http://shop.oreilly.com/product/0636920052289.do | Hands-on Machine Learning with Scikit-Learn and Tensorflow]] ([[https://proquest.safaribooksonline.com/9781491962282 | Full Text Online]]) ([[https://github.com/ageron/handson-ml | source code]])
* [[https://www.manning.com/books/deep-learning-with-python | Deep Learning with Python]] ([[https://proquest.safaribooksonline.com/9781617294433 | Full Text Online]]) ([[https://github.com/fchollet/deep-learning-with-python-notebooks | source code]])
* [[http://shop.oreilly.com/product/0636920065869.do | Tensorflow for Deep Learning]] ([[https://proquest.safaribooksonline.com/9781491980446 | Full Text Online]]) ([[https://github.com/matroid/dlwithtf | source code]])


### Courses

Python-based on-line data science training courses to dig deeper into a particular topic.

#### Udacity Nanodegree programs

* [[https://sa.udacity.com/course/ai-programming-python-nanodegree--nd089 | AI Programming with Python]]
* [[https://sa.udacity.com/course/data-scientist-nanodegree--nd025 | Become a Data Scientist]]
* [[https://sa.udacity.com/course/machine-learning-engineer-nanodegree--nd009 | Become a Machine Learning Engineer]]
* [[https://sa.udacity.com/course/deep-learning-nanodegree-foundation--nd101 | Deep Learning]]
* [[https://sa.udacity.com/course/natural-language-processing-nanodegree--nd892 | Natural Language Processing]]
* [[https://sa.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893 | Deep Reinforcement Learning]]

#### Coursera Specializations

* [[https://www.coursera.org/specializations/data-science-python | Applied Data Science with Python]]
* [[https://www.coursera.org/specializations/deep-learning | Deep Learning]]
* [[https://www.coursera.org/specializations/machine-learning-tensorflow-gcp | Machine Learning with TensorFlow on Google Cloud Platform]]
* [[https://www.coursera.org/specializations/advanced-machine-learning-tensorflow-gcp | Advanced Machine Learning with TensorFlow on Google Cloud Platform]]
* [[https://www.coursera.org/specializations/gcp-data-machine-learning | Data Engineering on Google Cloud Platform]]
* [[https://www.coursera.org/specializations/aml | Advanced Machine Learning]]
* [[https://www.coursera.org/specializations/genomic-data-science | Genomic Data Science]]

#### Others

* Various Deep and Machine Learning Courses from [fast.ai](https://www.fast.ai/).

