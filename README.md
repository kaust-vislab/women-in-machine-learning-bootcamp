# W2I-machine-learning-bootcamp
Workshop materials for Women 2 Impact: Machine Learning Bootcamp.

## 0. Install Git
Install the latest version of [Git](https://git-scm.com/downloads) version control system.

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
