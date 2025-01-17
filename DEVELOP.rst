===============
Developer Guide
===============

The project is written using `Sphinx`_ and `ReStructuredText`_.


Working on the project
======================

Python 3.7 is required.

Change into the ``docs`` directory:

.. code-block:: console

    $ cd docs

For help, run:

.. code-block:: console

    $ make

    Crate Docs Build

    Run `make <TARGET>`, where <TARGET> is one of:

      dev     Run a Sphinx development server that builds and lints the
              documentation as you edit the source files

      html    Build the static HTML output

      check   Build, test, and lint the documentation

      reset   Reset the build cache

You must install `fswatch`_ to use the ``dev`` target.


Continuous integration and deployment
=====================================

|build| |rtd|

This project uses GitHub Actions to run make check from the docs directory.

Also, Read the Docs automatically rebuilds the documentation whenever an active docs branch is updated.

To make changes to the RTD configuration (e.g., to activate or deactivate a release version), please contact an admin.

.. _fswatch: https://github.com/emcrisostomo/fswatch
.. _Read the Docs: http://readthedocs.org
.. _ReStructuredText: http://docutils.sourceforge.net/rst.html
.. _Sphinx: http://sphinx-doc.org/


.. |build| image:: https://img.shields.io/endpoint.svg?color=blue&url=https%3A%2F%2Fraw.githubusercontent.com%2Fcrate%2Fsql-99%2Fmaster%2Fdocs%2Fbuild.json
    :alt: Build version
    :target: https://github.com/crate/sql-99/blob/main/docs/build.json

.. |rtd| image:: https://readthedocs.org/projects/sql-99/badge/?version=latest
    :alt: Read The Docs status
    :scale: 100%
    :target: https://sql-99.readthedocs.io/en/latest/?badge=latest
