Groome-Python
=============

A [Groome](http://cjerdonek.github.com/groome/) project template for a
Python command-line script.

[This project is still under construction and is not yet usable.]


What is this?
-------------

The purpose of this project is to provide a Groome template to kick-start
a Python project.  The template is tailored to the following situation:

* a pure Python project (e.g. no C extensions) that
* exposes a command-line script,
* is written in Python 2 and supports Python 3, and
* uses Git for source control.

Rendered project features include--

* deployable to [PyPI](http://pypi.python.org/pypi) using
  [setup.py](http://docs.python.org/library/distutils.html),
* command-line interface via
  [argparse](http://docs.python.org/library/argparse.html),
* [logging](http://docs.python.org/library/logging.html) comes pre-configured,
* Python 3 supported via [2to3](http://docs.python.org/library/2to3.html),
* [unit tests](http://docs.python.org/library/unittest.html) and
  [doctests](http://docs.python.org/library/doctest.html) runnable with
  a single command,
* [tox](http://codespeak.net/tox/) support for running tests on all Python
  versions,
* [Travis CI](http://travis-ci.org/) support for continuous integration, and
* stubbed out license and documentation files.

Rendering the template creates a project that is working and ready-to-go
with respect to all of the above.

The project template is based on the structure of the code base for
[Molt](http://cjerdonek.github.com/molt/), which is the reference
implementation for rendering Groome templates.


Using the Project
-----------------

This section describes in more detail the project you get after rendering.

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
