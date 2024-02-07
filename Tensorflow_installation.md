## Tensorflow installation for MacOS M2 chip
###### 1. Install Homebrew (https://brew.sh/) if not installed yet.
###### 2. Install Xcode Command Line Tools
> xcode-select --install

###### 3. Install Miniforge
>1. go to https://github.com/conda-forge/miniforge install Miniforge
>2. select "yes" all the way until Miniforge installed.
>3. The "(base)" will show up in the front, for example: ***(base) amy@ MacBook-Pro ~ %***

###### 4. Create a virtual environment (name it envvv), and active the new created environment envvv
>conda create --name envv python=3.8

>conda activate envv

###### 5. Installing Tensorflow-MacOS
Install the Tensorflow dependencies:
>conda install -c apple tensorflow-deps

Install base TensorFlow:
>pip install tensorflow-macos

Install metal plugin:
>pip install tensorflow-metal

###### 6. Install Jupyter Notebook & Pandas
>conda install -c conda-forge -y pandas jupyter

###### 7. Run a script and Test
Install Tensorflow Datasets(if needed):
> pip install tensorflow_datasets

Open jupyter notebook
>jupyter notebook

It will open a browser window, run a script to test.


## Conda command should know
1. Set the conda's base environment not be activated on startup:
> $ conda config --set auto_activate_base false

2. To activate Conda environment:
> $ conda activate base

3. List all the conda environment
> $ conda env list

4. Activate a environment(base)
> $ conda activate base

5. Remove a conda environment - switch to another env(eg:base) then remove the specific env (eg: name is envv)
> $ conda activate base

> $ conda env remove --name envv

6. Switch back to system (local) environment
>$ conda deactivate


