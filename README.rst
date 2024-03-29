@@@@@@@@@@@@
easy-as-pypi
@@@@@@@@@@@@

.. .. image:: https://codecov.io/gh/pydob/easy-as-pypi/branch/develop/graph/badge.svg
..   :target: https://codecov.io/gh/pydob/easy-as-pypi
..   :alt: Coverage Status
..
.. .. image:: https://readthedocs.org/projects/easy-as-pypi/badge/?version=latest
..   :target: https://easy-as-pypi.readthedocs.io/en/latest/
..   :alt: Documentation Status
..
.. .. image:: https://img.shields.io/github/release/pydob/easy-as-pypi.svg?style=flat
..   :target: https://github.com/pydob/easy-as-pypi/releases
..   :alt: GitHub Release Status
..
.. .. image:: https://img.shields.io/pypi/v/easy-as-pypi.svg
..   :target: https://pypi.org/project/easy-as-pypi/
..   :alt: PyPI Release Status

.. image:: https://img.shields.io/github/license/pydob/easy-as-pypi.svg?style=flat
  :target: https://github.com/pydob/easy-as-pypi/blob/release/LICENSE
  :alt: License Status

One dev's boilerplate PyPI project.

.. Install with ``pip``::
..
..     pip3 install easy-as-pypi

########
Overview
########

Boilerplate for modern, bathroom-tub-included Python projects.

The boilerplate itself is installable and includes minimalist Click CLI.

But most of the gold is buried within:

- Modern Poetry and ``pyproject.toml`` setup.

- Supports cascading editable installs (install current project in
  editable mode, as well as any dependencies you might have source
  for locally; boilerplate manages alternative ``pyproject.toml``
  automatically).

- All the lints: ``black``, ``flake8``, ``isort``, ``pydocstyle``,
  ``doc8``, ``linkcheck``, ``poetry check``, and ``twine check``.

- Test against all active Python versions and lint using ``tox``.

- Run tasks, tests, and setup virtualenvs quickly using ``make``
  commands in your active virtualenv.

- Make commands to generate docs for *ReadTheDocs*.

- Make commands to localize user messages using ``Babel``.

- Make commands to setup and install to separate virtualenvs
  for various scenarios.

Most of the files are designed to be hard linked from the derived
projects themselves, as they won't need to be customized (such as
``Makefile``).

- That way when the boilerplate changes, you can just commit the
  changes in the derived project, call them "dependency updates"
  or something, and not have to worry about merging changes manually
  (and running ``meld`` or something).

