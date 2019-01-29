## Download Anaconda (A `.sh` file extension file for linux)
[a link](https://www.anaconda.com/download/)


## Install anaconda by running this file by
`$ bash Anaconda3-5.3.1-Linux-x86_64.sh`

## To know the version of your anaconda env
`$ conda -V`


## Create an environment by any name say `chatbot`
### python version 3.5 is preferred if you need to work with tensorflow
`$ conda create -n chatbot python=3.5 anaconda`


## Now activate your environment
`$ conda activate chatbot`
### Install Tensorflow in your environment(chatbot)
`$ pip3 install tensorflow==1.3.0`


## To list the environments 
`conda info --envs`

## Launch your Anaconda navigator in gui by
`$ anaconda-navigator`

## If some of your package is not opening. Please update your conda (first activate your environment in which you are working)
`$ conda update conda`
### More specifically
`$ conda update packageName`  e.g `spyder`


