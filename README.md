# Python Project Template
Template Python project for uploading the package to PyPi

## Start
1. Clone project:
```
git clone https://github.com/albertonarro/template-python-project-pypi.git
```

2. Create a virtual environment:
```
$ python3 -m venv env-dev
$ source env-dev/bin/activate
```

3. Install dev requirements:
```
$ python -m pip install -r dev-requirements.txt
```
4. Fill the project information in `setup.cfg`.
5. Start adding code inside the project_name folder.


## Usage
1. Update version in `setup.cfg`.
2. Build project:
```
$ python -m pip install build
```
3. Check the contents of the previously created `.whl` package:
```
$ check-wheel-contents dist/
```

4. Upload to PyPi:
```
$ twine upload dist/*
```

## Package installation
1. After uploading the package, you can install it by executing `pip install <project_name>`.
2. Package usage in python:
```python
>> import <folder_name>

>> from <folder_name> import <module>
```
