Groome-Python
=============

A [Groome](http://cjerdonek.github.com/groome/) project template for a
Python command-line script.

[This project is still under construction and not yet usable.]


What is this?
-------------

The purpose of this project is to provide a Groome template for a Python
project for the following situation:

* the package is pure Python (e.g. no C extensions)
* the project exposes a command-line script


Features
--------

This project template will have the following features:

* command-line help,

* options for verbose and silent output,

* automatic unit test and doctest discovery,

* use of Python's [unittest](http://docs.python.org/library/unittest.html)
  and [doctest](http://docs.python.org/library/doctest.html) modules, and

* integration of doctest with unittest via
  [doctest's unittest API](http://docs.python.org/library/doctest.html#unittest-api).

* TODO


Details
-------

Rendering the template with the sample configuration file generates a
project called "Pizza."  You can see this project in the expected directory.

The project exposes a command-line script which you can try by running
the following from the rendered project directory:

    $ python runpizza.py
    Output...
