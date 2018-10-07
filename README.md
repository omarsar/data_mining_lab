## Lab For Data Mining 2018 Fall Semester @ NTHU
This repository contains all the instructions and necessary code for Data Mining 2018 (Fall Semester) lab session.

---
### Computing Resources
- **Operating system:** Preferably Linux or MacOS. If you have Windows, things may crash unexpectedly (try installing a virtual machine if you need to)
- **RAM:** Minimum 8GB
- **Disk space:** Mininium 16GB

---
### Software Requirements
In this lab session we are going to be using Python as our main programming language. If you are not familiar with it, I recommend you start with this free [Python course](https://www.codecademy.com/learn/learn-python) offered by Codecademy. 

Here is a list of the required programs and libraries necessary for this lab session. (Please install them before coming to our lab session on Tuesday; this will save us a lot of time, plus these include some of the same libraries you may need for your first assignment).
- [Python 3+](https://www.python.org/download/releases/3.0/) (Note: lab and assignment will be done strictly using Python 3)
    - Install latest version of Python 3
- [Anaconda](https://www.anaconda.com/download/) (recommended but not required)
    - Install anaconda environment
- [Jupyter](http://jupyter.org/) Try to install the latest version and let it be compatible with your Python version. 
    - Install jupyter
- [Scikit Learn](http://scikit-learn.org/stable/index.html)
    - Install `sklearn` latest python library
- [Pandas](http://pandas.pydata.org/)
    - Install `pandas` python library
- [Numpy](http://www.numpy.org/)
    - Install `numpy` python library
- [Matplotlib](https://matplotlib.org/)
    - Install `maplotlib` for python
- [Plotly](https://plot.ly/)
    - Install and signup for `plotly`
- [NLTK](http://www.nltk.org/)
    - Install `nltk` library
---
### Test script
Open a jupyter notebook and run the following commands. If you have properly installed all the necessary libraries, you shouldn't have any problems running the lines of code below.
```python
# import library
import pandas as pd
import numpy as np
import nltk
from sklearn.datasets import fetch_20newsgroups
from sklearn.feature_extraction.text import CountVectorizer
import plotly.plotly as py
import plotly.graph_objs as go
import math
%matplotlib inline

# prepare dataset
categories = ['alt.atheism', 'soc.religion.christian', 'comp.graphics', 'sci.med']
twenty_train = fetch_20newsgroups(subset='train', categories=categories, shuffle=True, random_state=42)

twenty_train.data[0:5]
```
---
### Preview of Complete Jupyter Notebook (Coming Soon)

Please note that we will upload the jupyter notebook that will be used as guide on both this [Githug page](https://github.com/omarsar?tab=repositories) and our lab's [organization page](https://github.com/IDEA-NTHU-Taiwan). (**We will provide the link on the day of the lab session**). Additional instructions for assignments will be posted there, and submissions will more than likely be required to be posted through Github. In other words, if you don't have an account yet, please create a [Github](https://github.com/) account in advance. 

Don't worry! You will have plenty of time to learn Git before the assignment's due date. For the meanwhile, this [tutorial](https://tutorialzine.com/2016/06/learn-git-in-30-minutes) can help you get started with GitHub. Learning how to do version control and upload code using git will be useful for other courses in the future so if you want to take your skills to the next level, you can try this [online course](https://www.codecademy.com/learn/learn-git) offered by Codecademy. 

**One more thing:** I have setup a Slack page where we can engage (chat) or just in case anyone has any questions or concerns throughout the course. In Slack you can also setup private groups with your classmates and get to know each other better. From my experience, these tools are very helpful to get help from TAs and other classmates. This chat room will definitely be super helpful for when the project and exam time comes around. Come say :wave: if you are interested in joining the conversation. I will send an invite to your emails (provided by the iLMS). If you don't receive an invite by Sunday (07/10/2018) night, check your spam or send me your email again to ellfae@gmail.com.


---
### kaggle kernels

1. You need to create an account on kaggle (https://www.kaggle.com/).
2. Go to the Kernels page (https://www.kaggle.com/kernels), click `New Kernel` and choise `Notebook`.
3. Open the `Internet connected` in the Settings (right side).
4. Try our `Test script` code in the Notebook and run the code in a block by `shift + enter`.
5. If all the settings are correct, it would be like this:  

![kaggle kernels](https://i.imgur.com/xQ0VuOT.png)