---
layout: post
title: Install Anaconda and Torch on Linux (Python 3.4; Ubuntu 14.X 12.X; $USER directory)
---

Anaconda

wget https://3230d63b5fc54e62148e-c95ac804525aac4b6dba79b00b39d1d3.ssl.cf1.rackcdn.com/Anaconda3-2.3.0-Linux-x86_64.sh
bash Anaconda3-2.3.0-Linux-x86_64.sh
yes
$HOME/src/3rdparty/anaconda3
yes




Torch

Install dependencies

OpenBLAS
Append path to OpenBLAS library to LD_LIBRARY_PATH
export LD_LIBRARY_PATH="/home/jkim/src/3rdparty/OpenBLAS/0.2.13/lib;$LD_LIBRARY_PATH"

libreadline-dev
openssl libssl-dev
software-properties-common libgraphicsmagick1-dev nodejs libfftw3-dev sox libsox-dev libsox-fmt-all build-essential gcc g++ curl cmake libreadline-dev git-core libqt4-core libqt4-dev libjpeg-dev libpng-dev ncurses-dev imagemagick libzmq3-dev gfortran unzip gnuplot

git clone https://github.com/torch/distro.git ~/src/3rdparty/torch --recursive
cd ~/src/3rdparty/torch
./install.sh

