# Packaging Tutorial
* Author: https://github.com/shawlu95
* Project: https://github.com/shawlu95/packaging_tutorial
* Tutorial: https://packaging.python.org/tutorials/packaging-projects/
* Index: https://test.pypi.org/project/example-pkg-shawlu95/0.0.1/


### How to install
In Test PyPl repository
```bash

python3 -m pip install --upgrade twine

# upload
python3 -m twine upload --repository testpypi dist/*

# install
pip install -i https://test.pypi.org/simple/ example-pkg-shawlu95==0.0.1

python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps example-pkg-shawlu95
```

In production PyPl repository:
```bash
# upload
python3 -m twine upload dist/*

# install
python3 -m pip install [your-package].
```