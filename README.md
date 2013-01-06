Groome-Python
=============

A [Groome](http://cjerdonek.github.com/groome/) project template for a
Python command-line script.

[This project is still under construction and not yet usable.]


What is this?
-------------

The purpose of this project is to provide a Groome template to kick-start
a Python project.  The template is tailored to the following situation:

* the Python project is pure Python (e.g. no C extensions)
* the project should expose a command-line script

The rendered template is a ready-to-go, working project.

The project template is based on the structure of the code base for
[Molt](http://cjerdonek.github.com/molt/), which is the reference
implementation for rendering Groome templates.


Project Features
----------------

The project template comes with the following features already implemented:

* command-line argument parsing using
  [argparse](http://docs.python.org/2/library/argparse.html) with:
  * `--license` display license info
  * `-h, --help`
  * TODO
* ready to deploy to [PyPI](http://pypi.python.org/pypi) using
  [setup.py](http://docs.python.org/library/distutils.html)
* command-line help,

* options for verbose and silent output,

* automatic unit test and doctest discovery,

* use of Python's [unittest](http://docs.python.org/library/unittest.html)
  and [doctest](http://docs.python.org/library/doctest.html) modules, and

* integration of doctest with unittest via
  [doctest's unittest API](http://docs.python.org/library/doctest.html#unittest-api).

* TODO


Project Details
---------------

This section describes some of the details of the rendered project and how
to navigate around it once rendered.

Rendering the template with the sample configuration file creates a project
called "Pizza."  You can see this project in the project directory
`template/expected/`.

Pizza exposes a command-line script which you can run when developing
the following from the rendered project directory:

    $ python runpizza.py
    made pizza: ingredients

This is essentially a development convenience for running:

    $ python -m pizza.scripts.pizza
