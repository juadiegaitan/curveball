Installation
============

Curveball is a Python package. As such, it requires a Python interpreter to work. 
In addition, Curveball uses several scientific and data analysis libraries. 
All the dependencies are listed below, 
followed by a section containing instructions on how to install all the dependencies 
on the different operating systems.

Dependencies
------------

-  Python 2.7.x (2.6.x might work, 3.x to be supported soon)
-  numpy
-  scipy
-  pandas
-  matplotlib
-  seaborn
-  lmfit
-  statsmodels
-  sympy
-  xlrd
-  lxml
-  click

Users
------------

The recommended way to install the dependencies is to download and
install `Anaconda <https://www.continuum.io/downloads>`_, available for
Windows, OS X, and Linux.

After installing Anaconda, open a terminal or command line, and write the following commands to install the dependencies:

>>> conda update conda --yes
>>> conda install --yes requests pip numpy scipy matplotlib dateutil pandas statsmodels lxml seaborn sympy xlrd
>>> pip install lmfit

Then install Curveball (from `PyPi <https://pypi.python.org/pypi/curveball/>`_):

>>> pip install curveball


.. note::

	Another way to install Curveball is directly from `GitHub <https://github.com/yoavram/curveball>`_:

	>>> pip install git+https://github.com/yoavram/curveball.git

	or with a zip-file of Curveball, by running:

	>>> pip install <zip-file>

	replacing ``<zip-file>`` with the path to the zip-file.


Verify installation
^^^^^^^^^^^^^^^^^^^

To verify the installation, run this command:

>>> curveball --version
curveball, version x.x.x

where ``x.x.x`` will be replaced by the current version number (|release|).


.. note::

	To open a command line (or terminal) in:

	- **Windows**: click the *Start* button, type :command:`cmd.exe` and click *Enter*.
	- **Linux**: click *Ctrl-T*.
  	- **OS X**: search for :command:`terminal` in *Spotlight*.


Updating
^^^^^^^^

To update the depndencies installed with :command:`conda`, run:

>>> conda update <package-name>

replacing ``<package-name>`` with the name of the package you wish to update.

To update the packages installed with :command:`pip`:

>>> pip install --upgrade <package-name>

To update Curveball:

>>> pip install --upgrade curveball

Dependencies versions
^^^^^^^^^^^^^^^^^^^^^

The versions of the dependencies used to develop Curveball are documented in the `conda environment
file <https://github.com/yoavram/curveball/blob/master/environment.yml>`_.
However, this file includes packages that are not required for *running* Curveball.
Some packages are required to test Curveball and build the documents: for example, `nose`, `coverage`, and `sphinx`.

Note on :command:`conda` and :command:`pip`
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The same installation can be achieved using :command:`pip` instead of :command:`pip`, 
but on Windows and sometimes Linux and OS X, too, it is easier to use conda. 
Therefore, a :file:`requirements.txt` file is not provided.

Developers
--------------

Follow the `.travis.yml <https://github.com/yoavram/curveball/blob/master/.travis.yml>`_
file for a description of how to install Curveball and all the dependencies 
(including those required to test and build the docs) and how to run the tests using :command:`nosetests`.

Replace ``$TRAVIS_PYTHON_VERSION`` with the Python version you want (probably ``2.7.10``).

Contributing
^^^^^^^^^^^^

Please do! We encourage contributions, both to the documentation - 
from new sections and examples to typo fixes and rephrasing - 
and to the source code - 
from new file format parser to new growth and competition models.

Please see the `guidelines for contributing <https://github.com/yoavram/curveball/blob/master/CONTRIBUTING.md>`_
for instructions and best practices and feel free to contact me via 
`Email <mailto:yoav@yoavram.com>`_, `Twitter <https://twitter.com/yoavram>`_, and `Gitter <https://gitter.im/yoavram/curveball>`_