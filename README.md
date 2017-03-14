Tools and software library developed by the ONT Applications group
==================================================================


Installation
------------

Set up a virtual environment 

```
virtualenv  --system-site-packages wub_env
source wub_env/bin/activate
pip install --upgrade pip
pip install requests[security]
```

Then install the package via pip:

```
pip install git+https://github.com/nanoporetech/wub.git
```

If you installed the package in a virtual environment then do not forget to
load it before using the package:

```
source wub_env/bin/activate
```

Run the following to leave the virtual environment:

```
deactivate
```

You can also clone the repository and install using `setup.py`:

```
git clone https://github.com/nanoporetech/wub.git
cd wub
python setup.py install
```

Install the package in developer mode:

```
python setup.py develop
```

Run the tests:

```
make test
```

Build the documentation:

```
make docs
```

Issue `make help` to get a list of `make` targets.

Contributing
------------

- Please fork the repository and create a merge request to contribute.
- Please respect the structure outlined in `scripts/_template_script.py` from command line tools so documentation can be generated automatically.
- All non-trivial functions should have at least one test (with the exception of plotting functions).
- Use your best judgement when deciding whether to put a piece of code in a script or make it more reusable by incorporating it into the module.
- Use [bumpversion](http://bit.ly/2cSUryt) to manage package versioning.
- The code should be [PEP8](https://www.python.org/dev/peps/pep-0008) compliant, which can be tested by `make lint`.

TODO
----
- Add documentation link.

### What is a wub anyway?

It's a short, memorable name not on pypi yet. 
