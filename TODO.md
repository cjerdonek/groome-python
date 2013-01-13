TODO
====

Milestones
----------

* Flesh out the "expected" project in `template/expected`.  Use Molt as the
  model project and refactor Molt when I see that improvements can be made.

Tasks
-----

* Get long_description converted to ReST in setup.py.
* Stub out README.
* Stub out HISTORY.
* Stub out TODO.
* Rename setup\_description.rst to setup\_long_desc.rst.
* Add to setup_description.rst header comment that the file is the
  long_description argument to setup.py's setup().  It should be checked
  into source control and be part of the distribution so that setup()
  can be passed the long_description argument even without pandoc (i.e.
  for non-maintainers, etc).
* Add initial 2to3 support.
* Add an image to the README.
* Continue going through setup.py.
* Try using GitHub task lists:
  https://github.com/blog/1375-task-lists-in-gfm-issues-pulls-comments
* Get --run-tests running one substantive test.
* Remove the project_types/default after checking for useful code.
* Think about what should go in pizza_setup/ and what should go in a
  separate tools/ directory (or library).
* Look into how to download developer-specific dependencies.

* Switch config file from .json to .yaml.
* Add the ability to execute a script after rendering.
* Add an image to the README.
