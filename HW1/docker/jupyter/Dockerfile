FROM python:3.10-buster

RUN python -m pip install --upgrade pip
RUN pip install jupyterlab
COPY ./homework1/requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt

WORKDIR /notebooks

ENTRYPOINT jupyter-lab . --port=5000 --ip=0.0.0.0 --allow-root
