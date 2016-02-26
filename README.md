# Kocaeli

Docker container with a bootstrapped [anaconda](https://store.continuum.io/cshop/anaconda/) installed and ready to use.

This installs whole anaconda python distribution (with native python in 2.7 version) into the ``/opt/conda`` environment
and ensures that the default user has ``conda`` tool on their path.


Usage
-----
You can download and use this image by pulling it:

    docker pull ataniazov/kouintro2db
    docker run -i -t ataniazov/kouintro2db /bin/bash

