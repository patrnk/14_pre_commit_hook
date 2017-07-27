# Quadratic Equations Solver

A small module that enables you to solve quadratic equations with real roots automatically.

# How to Use

Import `quadratic_equation` module and use `get_roots` function:
```
$ python3
>>> from quadratic_equation import get_roots
>>> get_roots(1, 2, -3)
(-3.0, 1.0)
>>>
```

The function returns a tuple of real roots. The first root in the tuple is always less than the second. If the equation has only one real root, the second root in the tuple is None. If the equation has no real roots, `(None, None)` is returned.

# How to Launch Tests

```bash
python tests.py
```

# How to Activate Pre-Commit Hook

The included `pre-commit` file can only be run on Unix.

The included `pre-commit` script aborts the commit if any of the tests fail. To activate it, copy the file `pre-commit` into `.git/hooks` directory of the project. To bypass the activated script, run `git commit --no-verify`.

Depending on your [git config](https://stackoverflow.com/questions/23667859/why-is-git-clone-changing-file-permissions), you might want to make the `pre-commit` file executable:
```
$ chmod +x pre-commit
```

It is important to make sure that `python` command runs Python 3. Thus, don't forget to activate your virtual environment.

# Project Goals

The code is written for educational purposes. Training course for web-developers - [DEVMAN.org](https://devman.org)
