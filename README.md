## Udacity AWS Machine Learning Foundations Course Notes

### Python:
- Vectorization over looping
    - use numpy and set to optimise
- pip is a package manager for python (like npm)
- Testing
  - Make sure that pytest is installed (only once if you have not installed it)
    pip install -U pytest
  - name test file with 'test_'
  - also name each test def with 'test_'
  - to run test in 
  
### Making and installing a package
1. Create __init__.py file inside the code folder (e.g. 'distributions' folder) <br />
   code inside the init file (example) ```from .Gaussiandistribution import Gaussian```

2. Create setup.py (This file is required for pip install) in the same level as the code folder (e.g. 'distributions').

    code inside the setup file (example):
    ```
    setup(name='distributions',
          version='0.1',
          description='Gaussian distributions',
          packages=['distributions'],
          zip_safe=False)
    ```

3. To install the package

    ```pip install .``` in the same folder where setup.py file is located.
  
### Python Virtual Environment
1. To create a virtual evnironment

    ```python -m venv venv_name``` * replace 'venv_name' with any name.
    This will create a virtual environment folder in the current path.

2. To activate the virtual environment <br />
    ```source venv_name/bin/activate``` * use your own environment name here.

3. To come out of the virtual environment <br />
    ```deactivate```

