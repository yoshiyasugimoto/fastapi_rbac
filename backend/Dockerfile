FROM python:3.13

WORKDIR /app

ENV POETRY_HOME=/etc/poetry
RUN curl -sSL https://install.python-poetry.org | python -
ENV PATH $POETRY_HOME/bin:$PATH
RUN poetry config virtualenvs.create false


COPY . /app/
RUN poetry install --no-root