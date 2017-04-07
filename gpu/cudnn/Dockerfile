#ubuntu16.04
#karas = 2.0.1
#theano = 0.9
#gpu cuda8.0 & cudnn5.1

FROM citcailearning/scipy_gpu_cudnn_notebook:cuda8.0

MAINTAINER Mad Chang <citcailearning@gmail.com>

RUN /opt/conda/bin/pip install keras==2.0.1
COPY keras.json /home/$NB_USER/.keras/
RUN echo "[global]\ndevice=gpu\nfloatX=float32\noptimizer_including=cudnn\n[lib]\ncnmem=0.1\n[nvcc]\nfastmath=True\n[dnn]\nenabled=True" > /home/$NB_USER/.theanorc

USER $NB_USER
