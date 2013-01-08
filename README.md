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

Rendering the template creates a working project that is ready-to-go.


Project Features
----------------

The project template comes with the following features already implemented:

* command-line support using
  [argparse](http://docs.python.org/library/argparse.html).
  Initial supported options include:
  * `--license` display license info
  * `-h, --help`
  * TODO
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

This section describes details of the project you get when rendering.

The project template is based on the structure of the code base for
[Molt](http://cjerdonek.github.com/molt/), which is the reference
implementation for rendering Groome templates.

For discussion purposes, we will use the project created from the sample
configuration file.  This project is called "Pizza."  You can see it in
the `template/expected` directory of a source checkout.

Pizza exposes a command-line script which you can run as follows:

    $ python runpizza.py tomatoes garlic
    input: tomatoes, garlic

This is essentially a development convenience for running:

    $ python -m pizza.scripts.pizza ...

To get help and see all options:

    $ python runpizza.py -h


Project Organization
--------------------

    pizza/
        scripts/
            # specific to command-line usage (i.e. not needed for API).
            pizza/
