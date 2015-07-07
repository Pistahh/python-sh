[![Build Status](https://travis-ci.org/amoffat/sh.svg?branch=master)](https://travis-ci.org/amoffat/sh) [![Coverage Status](https://coveralls.io/repos/amoffat/sh/badge.svg?branch=master&service=github)](https://coveralls.io/github/amoffat/sh?branch=master)

[![Version](https://img.shields.io/pypi/v/sh.svg)](https://pypi.python.org/pypi/sh) [![Downloads](https://img.shields.io/pypi/dd/sh.svg)](https://pypi.python.org/pypi/sh)

sh (previously [pbs](http://pypi.python.org/pypi/pbs)) is a full-fledged
subprocess replacement for Python 2.6 - 3.4, PyPy and PyPy3
that allows you to call any program as if it were a function:

```python
from sh import ifconfig
print ifconfig("eth0")
```

sh is not a collection of system commands implemented in Python.

# Installation

    $> pip install sh

# Complete documentation @ http://amoffat.github.com/sh


# Testing

First install the development requirements:

    $> pip install -r requirements-dev.txt

Then run the tests like this:

    $> python sh.py test

To run a single test for all environments:

    $> python sh.py test FunctionalTests.test_unicode_arg
