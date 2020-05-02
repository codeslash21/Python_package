# Python_package
This project is the part of the Machine Learning Engineering Nanodegree program. In this project we create `distributions`
which can be uploaded to PyPi regular repository. This package has three modules. A testfile is there for unit testing.


## Getting Started:
`binomial_distribution_package` folder has `setup.py` file which contains metadata about the `distributions` package. In `distributions` package we have three modules and `__init__.py` files which tells python that this folder contains package. 

- **To run the unit tests:**

    >Go to `binomial_distribution_package` directory where `binomial_test.py` file exists.</br>
    >Run the command `python binomial_test.py` to run the unit tests.
  If all the test pass you get success messages. Its recomended to run the unit tests before publishing packages.
  
- **To upload package:**
To upload a python package to [PyPi](https://pypi.org/) regular repository you have to register. After register do the following - 

  **1.** Go to `binomial_distribution_package` directory where `setup.py` file exists.
  **2.** Run `python setup.py sdist` to generate required folders to upload the package. This command create a dist folder which contains a `jar.gz` file, this file contains the package.
  **3.** Run `pip install twine` to install `twine`. Its required to upload package.
  **4.** Run `twine upload dist/*` to upload the package to the `pypi` regular directory. If you want to upload to the `pypi` test directory then run `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`.
  **5.** After uploading to the `pypi` regular directory you can install the package using `pip` command like `pip install distributions`.
  
  
  ### License:
  This project is under _MIT License_ see here for more details [LICENSE](https://github.com/codeslash21/Python_package/blob/master/LICENSE)
