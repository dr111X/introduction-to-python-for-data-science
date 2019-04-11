[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kaust-vislab/introduction-to-python-for-data-science/fall-2019)

# Python for Data Science Workshop (Fall 2019)

## Installation Instructions

Install [Git](https://github.com/kaust-vislab/introduction-to-git-for-data-scientists#installation-instructions) so that you can [clone the repository](https://help.github.com/en/articles/cloning-a-repository) for the workshop onto your local machine.

To clone this repository open a terminal (or Git Bash shell if you installed Git on Windows), change the current working directory to the location where you want to create the clone of this repository and then run the following command in the terminal.

```bash
$ git clone https://github.com/kaust-vislab/introduction-to-python-for-data-science.git
```

### Using Docker

[Download and install Docker CE](https://hub.docker.com/search/?type=edition&offering=community) for you OS. In order to download Docker CE you will need to setup an account with [DockerHub](https://hub.docker.com/). Once you are logged into DockerHub and have downloaded and installed Docker CE, then you can run a container with all of the required software for the workshop properly installed and configured by running the following commands in the terminal.

```bash
$ cd introduction-to-python-for-data-science/
$ docker container run --rm -v $(pwd):/home/al-khawarizmi/project -p 8888:8888 -it kaustvl/introduction-to-python-for-data-science:fall-2019
```

Inside the container the Conda environment will already be activated so you can just launch the JupyterLab server as follows.

```bash
> jupyter lab --ip 0.0.0.0 --no-browser
```

Finally open a browser on your local machine and copy and paste the provided url.

### Without using Docker

Install the Python 3 version of [Miniconda](https://docs.conda.io/en/latest/miniconda.html) from Anaconda for your OS. Once you have installed Conda on your local machine you can use Conda to create and activate the software environment for the workshop by running the following commands in the terminal.

```bash
$ cd introduction-to-python-for-data-science
$ conda env create -f environment.yml
$ conda activate introduction-to-python-for-data-science
```

Once the environment has been activated, then you can launch the JupyterLab server by typing the following command in the terminal.

```bash
$ jupyter lab
```

## Additional Resources

### Core Data Science tools

In addition to knowledge of Python an aspiring data scientist you should seek to develop proficiency in the following areas:

* Version control using [Git](https://git-scm.com/) and either [GitHub](https://github.com/) or [GitLab](https://about.gitlab.com/).
* SQL programming for extracting data from relational databases.
* The Unix shell for interacting with clusters in the cloud ([GCP](https://cloud.google.com/), [AWS](https://aws.amazon.com/), [Azure](https://azure.microsoft.com/en-us/), etc)
* Container-based work flows using [Docker](https://www.docker.com/) to enable your data science pipelines to run on your laptop, on cluster, even on HPC (without changing your code!).

In addition to the Python lessons that we will cover in the workshop, [The Carpentries](https://carpentries.org) have excellent introductory materials on [version control using Git](http://swcarpentry.github.io/git-novice), [Bash Shell]([http://swcarpentry.github.io/shell-novice) and [SQL](http://swcarpentry.github.io/sql-novice-survey) as well as a number of more [domain-specific data-science lessons](https://datacarpentry.org/lessons/) that are built on this tool stack. There is also a lesson on [Testing and Continuous Integration with Python](http://katyhuff.github.io/python-testing/) which covers how to build automated testing infrastructure for you research software and data analysis.

#### Jupyter Notebooks

Here are a few Jupyter notebook cheat sheets that I have encountered and found useful.

* [Anaconda Jupyter Notebook Cheatsheet](https://docs.anaconda.com/_downloads/JupyterLab-Notebook-Cheatsheet.pdf)
* [DataCamp Jupyter Notebook Cheatsheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Jupyter_Notebook_Cheat_Sheet.pdf])
* [JupyterLab: Evolution of the Jupyter Notebook](https://towardsdatascience.com/jupyter-lab-evolution-of-the-jupyter-notebook-5297cacde6b)

### Machine Learning and Deep Learning

The following is a non-exhaustive list of Python for data science books and courses that I have found useful in my career as a data scientist.  **If you have a good learning resource that is not listed here please share!**

#### Books

There are a number of excellent books available all of which have source code (i.e., Jupyter notebooks) available for download via GitHub. 

* [Python for Data Analysis, 2nd Edition](http://shop.oreilly.com/product/0636920050896.do) ([source code](https://github.com/wesm/pydata-book)) 
* [Python Data Science Handbook](http://shop.oreilly.com/product/0636920034919.do) ([source code](https://github.com/jakevdp/PythonDataScienceHandbook))
* [Hands-on Machine Learning with Scikit-Learn and Tensorflow](http://shop.oreilly.com/product/0636920052289.do)([source code](https://github.com/ageron/handson-ml))
* [Deep Learning with Python](https://www.manning.com/books/deep-learning-with-python) ([source code](https://github.com/fchollet/deep-learning-with-python-notebooks))
* [Tensorflow for Deep Learning](http://shop.oreilly.com/product/0636920065869.do) ([source code](https://github.com/matroid/dlwithtf))

#### Courses

Python-based on-line data science training courses to dig deeper into a particular topic.

##### Udacity Nanodegree programs

* [AI Programming with Python](https://sa.udacity.com/course/ai-programming-python-nanodegree--nd089)
* [Become a Data Scientist](https://sa.udacity.com/course/data-scientist-nanodegree--nd025)
* [Become a Machine Learning Engineer](https://sa.udacity.com/course/machine-learning-engineer-nanodegree--nd009)
* [Deep Learning](https://sa.udacity.com/course/deep-learning-nanodegree-foundation--nd101)
* [Natural Language Processing](https://sa.udacity.com/course/natural-language-processing-nanodegree--nd892)
* [Deep Reinforcement Learning](https://sa.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893)

##### Coursera Specializations

* [Applied Data Science with Python](https://www.coursera.org/specializations/data-science-python)
* [Deep Learning](https://www.coursera.org/specializations/deep-learning)
* [Machine Learning with TensorFlow on Google Cloud Platform](https://www.coursera.org/specializations/machine-learning-tensorflow-gcp)
* [Advanced Machine Learning with TensorFlow on Google Cloud Platform](https://www.coursera.org/specializations/advanced-machine-learning-tensorflow-gcp)
* [Data Engineering on Google Cloud Platform](https://www.coursera.org/specializations/gcp-data-machine-learning)
* [Advanced Machine Learning](https://www.coursera.org/specializations/aml)
* [Genomic Data Science](https://www.coursera.org/specializations/genomic-data-science)

##### Others

* Various Deep and Machine Learning Courses from [fast.ai](https://www.fast.ai/).

