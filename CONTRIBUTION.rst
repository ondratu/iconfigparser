Contribution
============


Tests
-----
``test`` command in setup.py run unittest and doctest automatically, you can
run unittest manually by next commands:

.. code:: sh

    # unittest (builtin)
    ~$ python -m unittest discover -v ./tests

    # pytest (extra module)
    ~$ pytest -v

    # doctest (builtin - not output means example codes are OK)
    ~$ python -m doctest extendparser/*.py

**pytest** package have many additional extensions so you can use that.
Next command check all .rst files, source code with pep8 and doctest checkers.

.. code:: sh

    # check code with pytest and pylint, mypy and doctest
    ~$ pytest -v --pylint --mypy --doctest-plus --doctest-rst
