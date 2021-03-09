FROM python
ENV POETRY_HOME="/home/poetry/.poetry" 
RUN apt update
RUN apt-get update \
    && apt-get install --no-install-recommends -y \
        curl \
        build-essential \
        flake8 \
        pylint3
RUN groupadd -g 1000 -r poetry && useradd -u 1000 -m -r -g poetry poetry
USER poetry
RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
RUN mkdir /home/poetry/code/
WORKDIR /home/poetry/code/
ENV PATH="$POETRY_HOME/bin:$VENV_PATH/bin:$PATH"
ENTRYPOINT python
