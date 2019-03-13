[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kaust-vislab/W2I-machine-learning-bootcamp/master?urlpath=lab)

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
