# Kocaeli University Computer Engineering Introduction to Databases jupyter notebook docker container.

Docker container with a bootstrapped [anaconda](https://store.continuum.io/cshop/anaconda/) and jupyter notebook installed and ready to use.

This installs whole anaconda python distribution (with native python in 2.7 version and ipython-sql module) into the ``/opt/conda`` environment
and ensures that the default user has ``conda`` tool on their path.

Usage
-----
You can download and use this image by pulling it:

    docker pull ataniazov/kouintro2db
    docker run -p 8888:8888 -i -t ataniazov/kouintro2db /bin/bash

To start jupyter notebook service type in container:

    ipython notebook --no-browser --ip=*
