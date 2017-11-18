.. _getting_started_python:

Getting started with Python
===========================

Why Python?
-----------

Python is one of the most popular programming languages around due to its:

- simple and easy to read syntax making it quick to learn
- huge range of packages allowing it be used for a huge range of applications
- active open community of developers
- use behind many of the most popular websites in the world (Google, YouTube, Instagram, Dropbox, Reddit)

It is widely regarded as the main language for machine learning and is gaining ground against R for its use in other forms of data analysis.

Getting Started
---------------

Each person has their own preferences when learning something new so the route advised below may not suit everyone.

#. `Install <installing_python_>`_ it on your machine
#. Start by `learning the basics <learning_python_basics_>`_ of the language and the syntax.
#. Familiarise yourself with the `Python packages <python_for_data_analysis_>`_ that will be useful for actuarial analyses
#. Force yourself to use it for some real work, something simple that you may normally have used Excel for
#. Learn some intermediate Python so that you can implement projects more efficiently
#. Read others code to understand how to get the most out of the language

Following the steps above should get you well on your way but don't stop there:

#. Seek out other Python users for tips
#. Look at projects available online for ideas
#. Join a local community (e.g PyData) to find Python users in your area and learn from them
#. Look at Kaggle competition entries and blogs
#. Follow leading Python data scientists on Twitter for ideas

.. _getting_help:

Getting help
------------

You will get stuck as with any new tool. Inevitably there will be someone who has experienced your issue before so persevere and google your way through it:

#. Search the web for answers - StackOverFlow is an amazing website for questions and dedicated volunteers to help solve issues. Usually someone will have already encountered your problem and someone else will have pointed out a solution.
#. Read the documentation - at least read the getting started guides for which ever area you are stuck on.
#. Don't go it alone - persuade someone else in your organisation to learn with you
#. Find someone in your organisation who can help

.. _installing_python:

Installing Python
-----------------

Windows does not come with Python by default. Linux and MacOS users already have Python on their machines. However the version installed may not be suited for scientific analysis.

The easiest way to get started is to install `Anaconda <https://www.anaconda.com/download/>`_, which at its core is a Python installation customised for scientific use with lots of bells and whistles that will be useful along the way. It isn't a single program which may confuse newcomers but a collection of tools which are most easily launched through the Anaconda Navigator (one of the programs installed).

Once Anaconda is installed you have several ways of actually writing code and running it:

#. Launch a Jupyter Notebook where code is written in cells and the output displayed below the cell
#. Launch Spyder for an Interactive Development Environment (IDE) similar to RStudio or Visual Studio.
#. Write code in any other compatible text editor or IDE

.. _learning_python_basics:

Learning the basics
-------------------

There are lots of websites offering free online courses covering the basics most of which allow you to run code in the browser so that you don't need to even worry about installing the software. Here are just a few:

- `Codecademy - Learn Python <https://www.codecademy.com/learn/learn-python>`_
- `Datacamp - Intro to Python for Data Science <https://www.datacamp.com/courses/intro-to-python-for-data-science>`_
- `Udacity - Programming Foundations with Python <https://www.udacity.com/course/programming-foundations-with-python--ud036>`_

Look for a course that covers topics such as Lists, Dicts, Functions, Loops and Classes.

.. _python_for_data_analysis:

Python for Data Analysis
------------------------

A lot can be done with just core Python but its real power comes from making use of all the optional Python packages (think libraries in R or toolboxes in MatLab) that will make your life much easier and allow you to concentrate on your analyses. The following packages are potentially useful across a wide range of actuarial projects:

- `Numpy <http://www.numpy.org/>`_ - a foundational package that most other scientific packages in Python utilise. It introduces an array data type and a whole set of functions and classes for working with them. This package makes array calculations to run extremely quickly as most of the underlying code is in C and makes use of Intel's math kernels. It is unlikely you will need to use Numpy directly, at least initially, as other packages are more useful but you should make note of the basics.
- `Pandas <http://pandas.pydata.org/>`_ - for working with data tables (importing, editing, grouping, pivoting, merging, joining, reshaping, time series). This makes working with actuarial data very straightforward and this fantastic package is extremely well documented with a `10 minutes in Pandas <http://pandas.pydata.org/pandas-docs/stable/10min.html>`_ section which gets you up and running quickly.
- `SciPy <https://www.scipy.org/>`_ - mathematics package covering integration, optimization, interpolation, linear algebra and statistics. Very useful especially the statistics classes and functions.
- `Matplotlib <https://matplotlib.org/>`_ - the standard plotting library for creating a wide range of plots. The documentation is a needs some work but it can do anything you need it to if you persevere.

There are many online courses that focus on Python for data science, for example:

- `Udacity - Intro to Data Analysis <https://www.udacity.com/course/intro-to-data-analysis--ud170>`_
- `edX - Python for Data Science <https://www.edx.org/course/python-data-science-uc-san-diegox-dse200x>`_
- `Coursera - Introduction to Data Science in Python <https://www.coursera.org/learn/python-data-analysis>`_

There are several good books that lay the foundations:

- `Python for Data Analysis, Wes McKinney <http://shop.oreilly.com/product/0636920023784.do>`_ - written by the main author of Pandas
- `Python Data Science Handbook, Jake VanderPlas <http://shop.oreilly.com/product/0636920034919.do>`_ - written by a widely regarded data scientist, the book is freely available online on `GitHub <https://github.com/jakevdp/PythonDataScienceHandbook>`_
