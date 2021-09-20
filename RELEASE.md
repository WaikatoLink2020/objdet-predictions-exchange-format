# PyPi

Preparation:

* increment version in `setup.py`
* commit/push all changes

Commands for releasing on pypi.org (requires twine >= 1.8.0):

```commandline
find -name "*~" -delete
rm dist/*
./venv/bin/python setup.py clean
./venv/bin/python setup.py sdist
./venv/bin/twine upload dist/*
```

# Github

Steps:

* start new release (version: `vX.Y.Z`)
* enter release notes, i.e., significant changes since last release
* upload `opex-X.Y.Z.tar.gz` previously generated with `setyp.py`
* publish


