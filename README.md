[![Donate via PayPal][donate-image]][donate-link]
[![Discord][discord-image]][discord-link]
[![Build][github-ci-image]][github-ci-link]
[![Coverage Status][codecov-image]][codecov-link]
[![PyPI Version][pypi-image]][pypi-link]
[![PyPI - Python Version][python-image]][pypi-link]
![License][license-image-mit]

# Soup Sieve

## Overview

Soup Sieve is a CSS selector library designed to be used with [Beautiful Soup 4][bs4]. It aims to provide selecting,
matching, and filtering using modern CSS selectors. Soup Sieve currently provides selectors from the CSS level 1
specifications up through the latest CSS level 4 drafts and beyond (though some are not yet implemented).

Soup Sieve was written with the intent to replace Beautiful Soup's builtin select feature, and as of Beautiful Soup
version 4.7.0, it now is :confetti_ball:. Soup Sieve can also be imported in order to use its API directly for
more controlled, specialized parsing.

Soup Sieve has implemented most of the CSS selectors up through the latest CSS draft specifications, though there are a
number that don't make sense in a non-browser environment. Selectors that cannot provide meaningful functionality simply
do not match anything. Some of the supported selectors are:

- `.classes`
- `#ids`
- `[attributes=value]`
- `parent child`
- `parent > child`
- `sibling ~ sibling`
- `sibling + sibling`
- `:not(element.class, element2.class)`
- `:is(element.class, element2.class)`
- `parent:has(> child)`
- and [many more](https://facelessuser.github.io/soupsieve/selectors/)


## Installation

You must have Beautiful Soup already installed:

```
pip install beautifulsoup4
```

In most cases, assuming you've installed version 4.7.0, that should be all you need to do, but if you've installed via
some alternative method, and Soup Sieve is not automatically installed for your, you can install it directly:

```
pip install soupsieve
```

If you want to manually install it from source, navigate to the root of the project and run

```
python setup.py build
python setup.py install
```

## Documentation

Documentation is found here: https://facelessuser.github.io/soupsieve/.

## License

MIT License

Copyright (c) 2018 - 2022 Isaac Muse <isaacmuse@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[bs4]: https://beautiful-soup-4.readthedocs.io/en/latest/#

[github-ci-image]: https://github.com/facelessuser/soupsieve/workflows/build/badge.svg?branch=master&event=push
[github-ci-link]: https://github.com/facelessuser/soupsieve/actions?query=workflow%3Abuild+branch%3Amaster
[discord-image]: https://img.shields.io/discord/678289859768745989?logo=discord&logoColor=aaaaaa&color=mediumpurple&labelColor=333333
[discord-link]:https://discord.gg/XBnPUZF
[codecov-image]: https://img.shields.io/codecov/c/github/facelessuser/soupsieve/master.svg?logo=codecov&logoColor=aaaaaa&labelColor=333333
[codecov-link]: https://codecov.io/github/facelessuser/soupsieve
[pypi-image]: https://img.shields.io/pypi/v/soupsieve.svg?logo=pypi&logoColor=aaaaaa&labelColor=333333
[pypi-link]: https://pypi.python.org/pypi/soupsieve
[python-image]: https://img.shields.io/pypi/pyversions/soupsieve?logo=python&logoColor=aaaaaa&labelColor=333333
[license-image-mit]: https://img.shields.io/badge/license-MIT-blue.svg?labelColor=333333
[donate-image]: https://img.shields.io/badge/Donate-PayPal-3fabd1?logo=paypal
[donate-link]: https://www.paypal.me/facelessuser
