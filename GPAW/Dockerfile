FROM continuumio/miniconda3

WORKDIR /workspace

RUN conda install conda-forge::libxc -y && \
    conda install conda-forge::blas -y && \
    apt-get update -y && \
    apt install gcc -y && \
    pip install git+https://gitlab.com/gpaw/gpaw.git && \
    yes | gpaw install-data .
