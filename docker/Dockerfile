FROM continuumio/miniconda3:4.5.11

LABEL maintainer="david.pugh@kaust.edu.sa"

# create a new user (defaults to 'al-khawarizmi')
USER root
ARG username=al-khawarizmi
ENV HOME /home/${username}
RUN useradd --create-home --home-dir $HOME ${username}

# switch to newly created user to avoid running container as root
USER ${username}
WORKDIR $HOME

# create a project directory within the user's home
ARG project=project
RUN mkdir $HOME/${project}
WORKDIR $HOME/${project}

# build the specified conda environment from a file (defaults to 'environment.yml')
ARG environment=environment.yml
COPY ${environment} .
RUN conda env create --file ${environment} && \
    conda clean -tipsy && \
    echo ". /opt/conda/etc/profile.d/conda.sh" >> ~/.bashrc && \ 
    echo "conda activate $(head -1 ${environment} | cut -d' ' -f2)" >> ~/.bashrc

RUN conda activate $(head -1 ${environment} | cut -d' ' -f2)

# copied from parent image so that entrypoint does not run as root!
ENTRYPOINT [ "/usr/bin/tini", "--" ]

CMD [ "jupyter", "lab", "--ip", "0.0.0.0", "--no-browser" ]
