[![Docker Pulls](https://img.shields.io/docker/pulls/kaixhin/cuda-torch-mega.svg)](https://hub.docker.com/r/kaixhin/cuda-torch-mega/)
[![Docker Stars](https://img.shields.io/docker/stars/kaixhin/cuda-torch-mega.svg)](https://hub.docker.com/r/kaixhin/cuda-torch-mega/)

docker-torch-mega
=================

Available from the Docker Hub as `kaixhin/cuda-torch-mega`.

Ubuntu Core 14.04 + [CUDA 7.5](http://www.nvidia.com/object/cuda_home_new.html) + [cuDNN v5](https://developer.nvidia.com/cuDNN) + [Torch7](http://torch.ch/) (including iTorch). Includes the following additional packages:

- [alewrap](https://github.com/Kaixhin/alewrap)
- [autograd](https://github.com/twitter/torch-autograd)
- [classic](https://github.com/deepmind/classic)
- [dataset](https://github.com/twitter/torch-dataset)
- [distlearn](https://github.com/twitter/torch-distlearn)
- [dpnn](https://github.com/Element-Research/dpnn)
- [ffmpeg](https://github.com/clementfarabet/lua---ffmpeg)
- [imagine-nn](https://github.com/szagoruyko/imagine-nn)
- [ipc](https://github.com/twitter/torch-ipc)
- [loadcaffe](https://github.com/szagoruyko/loadcaffe)
- [logroll](https://github.com/rosejn/logroll)
- [luaposix](https://github.com/luaposix/luaposix)
- [LuaSocket](https://github.com/diegonehab/luasocket)
- [Moses](https://github.com/Yonaba/Moses)
- [nccl](https://github.com/ngimel/nccl.torch)
- [nninit](https://github.com/Kaixhin/nninit)
- [nnquery](https://github.com/bshillingford/nnquery)
- [parallel](https://github.com/clementfarabet/lua---parallel)
- [rlenvs](https://github.com/Kaixhin/rlenvs)
- [rnn](https://github.com/Element-Research/rnn)
- [signal](https://github.com/soumith/torch-signal)
- [stn](https://github.com/qassemoquab/stnbhwd)
- [tds](https://github.com/torch/tds)
- [torchx](https://github.com/nicolas-leonard/torchx)
- [xitari](https://github.com/lake4790k/xitari)

Requirements
------------

- [NVIDIA Docker](https://github.com/NVIDIA/nvidia-docker) - see [requirements](https://github.com/NVIDIA/nvidia-docker/wiki/CUDA#requirements) for more details.

Usage
-----
Use NVIDIA Docker: ``nvidia-docker run -it kaixhin/cuda-torch-mega``.

For more information on CUDA on Docker, see [this readme](https://github.com/Kaixhin/dockerfiles#cuda).

To use Jupyter/iTorch open up the appropriate port. For example, use ``nvidia-docker run -it -p 8888:8888 kaixhin/cuda-torch-mega``. Then run `jupyter notebook --ip="0.0.0.0" --no-browser` to open a notebook on `localhost:8888`.
