Bootstrap:docker
From:nfcore/base

%labels
    MAINTAINER Peter Kruczkiewicz
    DESCRIPTION Singularity image containing all requirements for the peterk87/nf-villumina pipeline
    VERSION 2.0.0

%environment
    PATH=/opt/conda/envs/nf-villumina-2.0.0/bin:$PATH
    export PATH

%files
    environment.yml /

%post
    /opt/conda/bin/conda env create -f /environment.yml
    /opt/conda/bin/conda clean -a
