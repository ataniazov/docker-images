# Kocaeli University Computer Engineering Introduction to Databases jupyter notebook docker container.

Docker container with a bootstrapped [anaconda](https://store.continuum.io/cshop/anaconda/) and jupyter notebook installed and ready to use.

This installs whole anaconda python distribution (with native python in 2.7 version and ipython-sql module) into the ``/opt/conda`` environment
and ensures that the default user has ``conda`` tool on their path.

Usage
-----
You can download and use this image by pulling it:

    $ docker pull ataniazov/kouintro2db

If you are using **Linux** and have a
[Docker daemon running](https://docs.docker.com/installation/),
e.g. reachable on `localhost`, start a container with:

    $ docker run --rm -it -p 8888:8888 ataniazov/kouintro2db /bin/bash

In your browser, open the URL `http://localhost:8888/`.

On other platforms, such as **Windows and OS X**, that use
[`docker-machine`](https://docs.docker.com/machine/install-machine/) with `docker`, a container can be started using
`docker-machine`. In the browser, open the URL `http://ip:8888/` where `ip` is
the IP address returned from the command [`docker-machine ip <MACHINE>`](https://docs.docker.com/machine/reference/ip/):

    $ docker-machine ip <MACHINE>

For example,

    $ docker-machine ip myjupytermachine
    192.168.99.104

In browser, open `http://192.168.99.104:8888`.

NOTE: With the deprecated `boot2docker`, use the command `boot2docker ip` to
determine the URL.
