# scitemplate

If you don't already have twine installed run the following:
`python -m pip install --user --upgrade twine`

## The following will create the package
```
python setup.py sdist bdist_wheel
twine check dist/PROJECT_NAME.tar.gz
```

## Install to python environment localling

`pip install PATH_TO_PROJECT/dist/PROJECT_NAME.tar.gz`
You should run this before uploading it and check all works as expected.

## The following will push the package to pip 
**Note you need to set up a pip account first**

```
twine upload dist/*
```

## Have a look at your projects page on pip

`https://pypi.org/project/PROJECT_NAME/`
