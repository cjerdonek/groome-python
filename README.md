Groome-Python
=============

A [Groome](http://cjerdonek.github.com/groome/) project template for a
Python command-line script.

[This project is still under construction and not yet usable.]


What is this?
-------------

The purpose of this project is to provide a Groome template to kick-start
a Python project.  The template is tailor-made for the following situation:

* the Python project is pure Python (e.g. no C extensions)
* the project should expose a command-line script
* the project is written in Python 2 and supports Python 3 via
  [2to3](http://docs.python.org/library/2to3.html)

Rendering the template creates a working project that is ready-to-go.

The project template is based on the structure of the code base for
[Molt](http://cjerdonek.github.com/molt/), which is the reference
implementation for rendering Groome templates.


Project Features
----------------

The project template comes with the following features already implemented:

* command-line support using
  [argparse](http://docs.python.org/library/argparse.html).
  Initially implemented options include:
  * run project tests
  * display license info
  * display version info
  * display help
  * run in verbose mode
* ready to deploy to [PyPI](http://pypi.python.org/pypi) using
  [setup.py](http://docs.python.org/library/distutils.html)
* logging using the
  [logging](http://docs.python.org/library/logging.html) module,

* options for verbose and silent output,

* automatic unit test and doctest discovery,

* use of Python's [unittest](http://docs.python.org/library/unittest.html)
  and [doctest](http://docs.python.org/library/doctest.html) modules, and

* integration of doctest with unittest via
  [doctest's unittest API](http://docs.python.org/library/doctest.html#unittest-api).

* TODO


Project Details
---------------

This section describes the project you get after rendering in more detail.
For discussion purposes, we use the project created from the sample
configuration file.  However, all of the following still holds when using
your own configuration file (with appropriate substitution of names, etc).

The sample project is called "Pizza."  You can see it in the
`template/expected` directory of the source tree.

Pizza exposes a command-line script which you can run as follows:

    $ python runpizza.py tomatoes garlic
    input: tomatoes, garlic

This script is essentially a development convenience for running:

    $ python -m pizza.scripts.pizza ...

To get help and see all options:

    $ python runpizza.py --help

To run project tests (which are already stubbed out):

    $ python runpizza.py --run-tests


Project Organization
--------------------

    pizza/
        # command-line specific code (i.e. not needed for API).
        scripts/
            pizza/
        # test-specific code
        test/
            # test infrastructure and support code
            harness/
            # test modules in correspondence with package modules
            pizza/
    # Convenience wrapper to call main script while developing
    runpizza.py
