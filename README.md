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
* is written in Python 2 and supports Python 3,
* uses Git for source control, and
* could be potentially large or complex.

Features of the project after rendering include--

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

Rendering the template creates a project that is working and ready-to-go with
respect to all of the above.  The project template is based on the structure
of the code base for [Molt](http://cjerdonek.github.com/molt/), which is the
reference implementation for rendering Groome templates.


Using the Project
-----------------

This section describes how to start using the project you get after rendering.

For discussion purposes, we use the project created from the sample
configuration file.  However, all of this holds for any configuration file;
only the names will be different.  The sample project is called "Pizza."  You
can see it in the `template/expected` directory, which is a git submodule
that we maintain in a separate repo called
[groome-python-expected](https://github.com/cjerdonek/groome-python-expected).
It is an actual working project! :)

Check out the [Pizza](https://github.com/cjerdonek/groome-python-expected)
project page for details on what you get and how to use it.


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
