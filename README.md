[![PyPI version](https://badge.fury.io/py/pmdarima.svg)](https://badge.fury.io/py/pmdarima)
[![Linux build status](https://travis-ci.org/tgsmith61591/pyramid.svg?branch=master)](https://travis-ci.org/tgsmith61591/pyramid)
[![Windows build status](https://ci.appveyor.com/api/projects/status/592vawuu69kd6d21?svg=true)](https://ci.appveyor.com/project/tgsmith61591/pyramid)
[![PyPy build status](https://circleci.com/gh/tgsmith61591/pyramid.svg?style=svg)](https://circleci.com/gh/tgsmith61591/pyramid)
[![codecov](https://codecov.io/gh/tgsmith61591/pyramid/branch/master/graph/badge.svg)](https://codecov.io/gh/tgsmith61591/pyramid)
![Supported versions](https://img.shields.io/badge/python-2.7-blue.svg)
![Supported versions](https://img.shields.io/badge/python-3.5-blue.svg)
![Supported versions](https://img.shields.io/badge/python-3.6-blue.svg)

# pmdarima

Pmdarima (originally `pyramid-arima`, for the anagram) is a no-nonsense statistical Python library with a solitary objective: bring R's
[`auto.arima`](https://www.rdocumentation.org/packages/forecast/versions/7.3/topics/auto.arima)
functionality to Python. Pmdarima operates by wrapping
[`statsmodels.tsa.ARIMA`](https://github.com/statsmodels/statsmodels/blob/master/statsmodels/tsa/arima_model.py) and
[`statsmodels.tsa.statespace.SARIMAX`](https://github.com/statsmodels/statsmodels/blob/master/statsmodels/tsa/statespace/sarimax.py)
into one estimator class and creating a more user-friendly estimator interface for programmers familiar with scikit-learn.


## Installation

Pmdarima is on pypi under the package name `pmdarima` and can be downloaded via `pip`:

```bash
$ pip install pmdarima
```

Note that legacy versions (<1.0.0) are available under the name "`pyramid-arima`" and
can be pip installed via:

```bash
# Legacy warning:
$ pip install pyramid-arima
# python -c 'import pyramid;'
```

To ensure the package was built correctly, import the following module in python:

```python
from pmdarima.arima import auto_arima
```


### Availability

`pmdarima` is available in pre-built Wheel files for the following Python versions:

* Python 2.7:
  * Mac
  * Linux (manylinux)
  * Windows (32 & 64-bit)
* Python 3.5:
  * Mac
  * Linux (manylinux)
  * Windows (32 & 64-bit)
* Python 3.6:
  * Linux (manylinux)
  * Windows (32 & 64-bit)
  
If a wheel doesn't exist for your platform, you can still `pip install` and it will
build from the source distribution tarball.


### Documentation

All of your questions and more (including examples and guides) can be answered
by the [Pyramid documentation](https://www.alkaline-ml.com/pyramid). If not,
always feel free to file an issue.
