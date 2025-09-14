

# Install Instructions

1. Clone this repository
2. Install [uv](https://docs.astral.sh/uv/getting-started/installation/) and [brew](https://brew.sh/)
3. `brew install llvm` to get clang and co. 
4. Get the right python with `uv python install 3.9`
5. Run `uv python list` to find where this was installed to. It will be something like `~/.local/share/uv/python/cpython-3.9.0-macos-x86_64-none/bin/python3.9`.
6. In the root of this repository run 

```bash
CPPFLAGS="-I/<folder from above>/include/python3.9/" LDFLAGS="-L/<folder from above>/lib/" CXX=/usr/local/opt/llvm/bin/clang++ CC=/usr/local/opt/llvm/bin/clang uv sync
```

This will install everything. 

The inital run seems very slow, not entirely sure why. 

<hr />

# Velocyto [![Build Status](https://travis-ci.org/velocyto-team/velocyto.py.svg?branch=master)](https://travis-ci.org/velocyto-team/velocyto.py)

*This repo is not maintained anymore. Instead consider using [STARSolo](https://github.com/alexdobin/STAR/tree/master) which mimics velocyto behavior, is up-to-date, and quicker.*

This repo contains the source code for `the velocyto.py` library.

For more information consult the [velocyto.py documentation](http://velocyto.org/velocyto.py/index.html).