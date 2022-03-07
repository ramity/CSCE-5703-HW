FROM python:3.10-buster

RUN python -m pip install --upgrade pip
RUN pip install jupyterlab
RUN pip install numpy
RUN pip install matplotlib
RUN pip install opencv-python-headless
RUN pip install opencv-contrib-python-headless

WORKDIR /notebooks

ENTRYPOINT jupyter-lab . --port=5001 --ip=0.0.0.0 --allow-root
