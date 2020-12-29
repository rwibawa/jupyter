# Data Analysis with Python

## 1. Install `Anaconda` to set the workspace
Note: [anaconda vs miniconda](https://stackoverflow.com/questions/45421163/anaconda-vs-miniconda#:~:text=Anaconda%20is%20a%20full%20distribution,%2C%20its%20dependencies%2C%20and%20Python)

Download the ['64-Bit Command Line Installer (428 MB)' for Mac](https://www.anaconda.com/products/individual#macos)
```bash
$ cd ~/Downloads/
$ chmod +x Anaconda3-2020.11-MacOSX-x86_64.sh
$ ./Anaconda3-2020.11-MacOSX-x86_64.sh

# PREFIX=/Users/rwibawa/anaconda3
# modified      /Users/rwibawa/.bash_profile

# ==> For changes to take effect, close and re-open your current shell. <==

# If you'd prefer that conda's base environment not be activated on startup, 
#    set the auto_activate_base parameter to false: 

# conda config --set auto_activate_base false

# Thank you for installing Anaconda3!

$ export=/Users/rwibawa/anaconda3/bin:$PATH
```

## 2. install `tensorflow`
* [Tutorial](https://stackoverflow.com/questions/63111115/unable-to-install-tensorflow-using-conda-with-python-3-8)
```bash
$ conda create -n p37env python=3.7
$ conda activate p37env

$ conda search tensorflow
$ conda install tensorflow

$ conda deactivate
```

## 3. Use `jupyter notebook`
* [Tutorial](https://www.dataquest.io/blog/jupyter-notebook-tutorial/)
```bash
$ conda search jupyter
$ conda install jupyter
$ pip install jupyter_contrib_nbextensions && jupyter contrib nbextension install

$ conda install seaborn
$ jupyter notebook &
```

### Notebooks:
* [Learn Jupyter Notebook](note_01/learn%20Jupyter%20Notebook.ipynb)
* [Learn Machine Learning](ml_01/Learn%20Machine%20Learning.ipynb)
* [Learn Tensor Flow](tensorflow_01/beginner.ipynb)