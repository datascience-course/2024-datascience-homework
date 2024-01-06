# Homework 0
**Introduction to Data Science - MATH 4100 / COMP 5360.**  
*This homework is due by January 12th, 11:59pm*  


Welcome to MATH 4100 and Computing 5360 – Introduction to Data Science. In this class, we will be using a variety of tools that will require some initial configuration. To ensure everything goes smoothly moving forward, we will set up the majority of those tools in this homework. This homework will not be graded, but **it is essential that you complete it before the second lecture** as it sets up the tools that we will be using in class for exercises.

## 1. Setup

We'll often work on practical skills related to data science. That means we'll write code, and we'll do that in a programming language called Python.

Python has three advantages for this class: it's pretty easy to learn, it's the language of choice for many data scientists, and it can be used inside of Jupyter Notebooks – more on the latter will follow later.

We also assume that you know the basics of how to work with a terminal / console. If you don't check out an introduction like [this](http://tutorial.djangogirls.org/en/intro_to_command_line/).  

First, we'll need to install some things:

### 1.1 Installing Python

Chances are, if you're on a mac, you already have Python installed. You can simply try to run python from a console by running

```
$ python
```

However, as most software, Python comes in different versions and is packaged differently depending on your needs. In this class we'll use a Python distribution called Anaconda. Anaconda comes with a lot of packages that we'll need, so it is the most hassle-free option for us.

Go to [this website](https://www.anaconda.com/download/) and install anaconda for Python 3.11 for your operating system. [Here](https://docs.continuum.io/anaconda/install) are installation instructions if you need them. If you already have anaconda installed, please make sure that you're using the latest version or [update](http://docs.continuum.io/anaconda/install/update-version/) if necessary. For example on a Mac anaconda can be updated to the most recent version (2023.09-0) by entering the following commands in the command line:

```
$ conda update conda
$ conda install anaconda=2023.09-0
```

You'll have to create a new environment for Python 3.11 if you're not using that already. If you did a fresh install, this won't be necessary. Here is the update command:

```
$ conda install python=3.11
```

Once you've installed Anaconda, close your terminal window and re-open it - otherwise your terminal won't recognize the Anaconda commands.

Anaconda is both, a package manager and an environment manager. A package manager manages, well, packages. Packages add specific pieces of functionality - there are packages for web scraping, or for data visualization, for example. An environment manager, in contrast, allows you to have different versions of packages installed at the same time. We'll dive into environments and packages when we need them at a later point.

Let's see whether Anaconda works as intended. Run:

```
$ conda --version
```

from your terminal. You should see something like this as a result:

```
$ conda --version
conda 23.7.4 
```

Similarly, for python, you should see something like this:

```
$ python --version
Python 3.11.5
```

Note that all of these commands can be done through the Anaconda Navigator itself. To do so, go to the "Environments" tab on the left-hand side of Anaconda Navigator. From there, you can search for python (or any of the other packages installed) and the version will be clearly indicated.

You can also check out the [official website](http://conda.pydata.org/docs/test-drive.html) for more details on anaconda, environments, and packages.

### 1.2 Installing Jupyter Notebooks

***Check out the official Jupyter Notebooks documentation [here](http://jupyter.readthedocs.io/en/latest/index.html) for all the details***

We'll be running Python through Jupyter Notebooks as they are great for the data science process and for teaching, but you should be aware of the other options we discuss here.

Notebooks are stored in files that end with a `.ipynb` extension. They are included in the [basic-python](https://github.com/datascience-course/2024-datascience-homework/tree/main/HW0/basic-python) folder in this directory. Download them and save them to a folder.

Notebooks make use of an improved, interactive client for python called [IPython](https://ipython.org/). IPython might already be installed in the latest version if you did a clean anaconda install. To check, we'll use anaconda to install the proper version of IPython. Run:

```
$ conda install ipython
```

and confirm that in fact ipython 7.31.* is installed.
```
$ ipython --version
8.15.0
```

Now, change directories in your console so that you're in the directory where the notebook file is saved and run:

```
$ jupyter notebook
```

This will start the notebook server and should open up a browser window point to [http://localhost:8888/](http://localhost:8888/) that will look like that:

![Jupyter Notebook Screenshot](jupyter.png)

Click on the `02-notebooks.ipynb` entry to see if it works. We'll take it from there in the labs!

### 2. Self Study: Python

We recommend that you go through [Google's Python Tutorial](https://developers.google.com/edu/python), sections Intro, Strings, Lists, Sorting, Dicts and Files. 
