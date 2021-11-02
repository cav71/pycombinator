release process
---------------

Generate intial entry in pypi.org
    pip install build twine

    python -m build .
    twine upload --repository pypi dist/*


* https://packaging.python.org/tutorials/packaging-projects
