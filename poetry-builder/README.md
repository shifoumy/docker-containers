Poetry Builder Base Image
------------------------------

From python latest tag image, it will install poetry from shell script according to documentation : https://python-poetry.org/docs/#osx-linux-bashonwindows-install-instructions

`poetry` user is created and used to execute.

Working directory is created at `/home/poetry/code/`.

Poetry binary installed at `/home/poetry/.poetry/bin`

Entrypoint is set to `poetry` command

Usages:
-------

Build image :
=============
`docker build -t my_tag:version .`

Run container :
===============
`docker run -v [path to your project]:/home/poetry/code/ ashamss/poetry [poetry cmd]`
