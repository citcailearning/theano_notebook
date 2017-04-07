#karas = 2.0.1
#theano - 0.9
#use cpu

FROM citcailearning/scipy_notebook:ubuntu16.04

MAINTAINER Mad Chang <citcailearning@gmail.com>

RUN /opt/conda/bin/pip install keras==2.0.1
COPY keras.json /home/$NB_USER/.keras/

USER $NB_USER
