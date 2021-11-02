---------------
Release process
---------------
These are the instructions to initially create a first package release
on `PyPI`_ (TBD `conda-forge`_).
Once the first release (eg. 0.0.0) landed in `PyPI`_ subsequent releases
will be automated. 


First package release
~~~~~~~~~~~~~~~~~~~~~

Prerequisites
-------------

Initially you need to create a pair of \*.whl, \*.tar.gz files: in order to do that 
you need an environment with at least these few packages::

    pip install twine setuptools-github
    or
    conda install twine setuptools-github

Generate intial packages and install them in pypi::
        
        python -m build .
        twine upload --repository pypi dist/*


.. _`packaging`:  https://packaging.python.org/tutorials/packaging-projects
.. _`pip`: https://pypi.org/project/pip/
.. _`PyPI`: https://pypi.org/project
.. _`conda-forge`: https://conda-forge.org
