---
layout: post
title: Install Anaconda and Torch on Linux (Python 3.4; Ubuntu 14.X 12.X; $USER directory)
---

OpenBLAS
Append path to OpenBLAS library to LD_LIBRARY_PATH
export LD_LIBRARY_PATH="/home/jkim/src/3rdparty/OpenBLAS/0.2.13/lib:$LD_LIBRARY_PATH" # do this at the end of .bashrc


Anaconda

wget https://3230d63b5fc54e62148e-c95ac804525aac4b6dba79b00b39d1d3.ssl.cf1.rackcdn.com/Anaconda3-2.3.0-Linux-x86_64.sh
bash Anaconda3-2.3.0-Linux-x86_64.sh
yes
$HOME/src/3rdparty/anaconda3
yes

conda remove atlas
#conda install -c https://conda.anaconda.org/jakirkham openblas
echo -e "\n[blas]\nldflags = -lopenblas -lgfortran\n" >> ~/.theanorc
#conda remove openblas


Torch

Install dependencies

libreadline-dev
openssl libssl-dev
software-properties-common libgraphicsmagick1-dev nodejs libfftw3-dev sox libsox-dev libsox-fmt-all build-essential gcc g++ curl cmake libreadline-dev git-core libqt4-core libqt4-dev libjpeg-dev libpng-dev ncurses-dev imagemagick libzmq3-dev gfortran unzip gnuplot

git clone https://github.com/torch/distro.git ~/src/3rdparty/torch --recursive
cd ~/src/3rdparty/torch
./install.sh



c.NotebookApp.password = u'sha1:8b7193c63f29:0acb2921be75ccf40cbf4232e8518c2fe2412ce9'
c.NotebookApp.ip = '192.168.70.84'
c.NotebookApp.port = 8888
c.NotebookApp.notebook_dir = '/home/jkim/src/python'
c.NotebookApp.open_browser = False





CPLUS_INCLUDE_PATH=/home/jkim/src/3rdparty/OpenBLAS/0.2.13/include LDFLAGS="-L/home/jkim/src/3rdparty/OpenBLAS/0.2.13/lib" pip install tsne









