[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kaust-vislab/W2I-machine-learning-bootcamp/master)

# W2I-machine-learning-bootcamp
Workshop materials for Women 2 Impact: Machine Learning Bootcamp.

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

# Recommended installation instructions

## 1. Install Anaconda
Install the Python 3.7 version of either [Anaconda](https://www.anaconda.com/distribution/) or [miniconda](https://docs.conda.io/en/latest/miniconda.html). 

## 2. Clone the workshop repository using Git

```bash
$ git clone https://github.com/kaust-vislab/W2I-machine-learning-bootcamp.git
```

## 3. Create the Conda environment 
Change into the workshop directory and create the conda environment.

```bash
$ cd W2I-machine-learning-bootcamp/
$ conda env create -f environment.yml
```

## 4. Activate the Conda environment

```bash
$ source activate W2I-machine-learning-bootcamp
```

## 5. Start JupyterLab

```
$ jupyter lab
```

# Optional installation instructions

## 1. Install Docker CE
Sign up for an account on [DockerHub](https://hub.docker.com) and install the version of [Docker CE](https://hub.docker.com/search/?type=edition&offering=community) for your operating system.

## 2. Run a Docker container with the required software pre-installed

```bash
$ cd W2I-machine-learning-bootcamp/
$ docker-compose up
```

When you are finished with your work you may want to run 

```bash
$ docker-compose down
```

to gracefully tear down the running container.
