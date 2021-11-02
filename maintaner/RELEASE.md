Release process
---------------

## In the master branch
Make sure the master branch is building.

1. Generate intial entry in pypi.org

        pip install build t
        wine
2. Publish the package in the testpypi or pypi repository
        
        python -m build .
        twine upload --repository pypi dist/*

## Notes
* https://packaging.python.org/tutorials/packaging-projects
