# penguin-devops
Lab solutions for the book [DevOps for Data Science](https://do4ds.com/)

## Virtual Environment Setup

The project uses venv and renv for Python and R respectively.


### Virtual environment for Python

The python virtual environment is created using the `venv` module. An environment with the name `.venv` has been created in the root directory of the project by running the following command:

```bash
python3 -m venv .venv
```

To activate the virtual environment (in Powershell), run the following command:

```Powershell
.venv\Scripts\Activate.ps1
```

To install the required packages listed in the requirements.txt file, run the following command:

```bash
pip install -r requirements.txt
```

To deactivate the virtual environment, run the following command:

```bash
deactivate
```

### Updating the requirements.txt file

If you want to update the requirements.txt file with the packages installed in your virtual environment, you can run the following command:

```bash
pip freeze > requirements.txt
```
This will overwrite the existing requirements.txt file with the current packages installed in your virtual environment.

The Python documentation is a good place to consult in case you run into obstacles. You can find it [here](https://docs.python.org/3/library/venv.html).

### Virtual environment for R

The R virtual environment is created using the `renv` package. Renv stores the dependencies in a renv.lock file. 

If you want to install the packages listed in the `renv.lock` file, you can run the following command:

```r
renv::restore()
```

Please consult the [renv documentation](https://rstudio.github.io/renv/articles/renv.html) for more information on how to use renv.

## Running the Shiny App

After starting the Python virtual environment, you can run the Shiny app by running the following commands in the terminal:

```bash
py
from shiny import run_app
run_app()
```

This will start the `app.py` in the working directory. After running the app, you can close the app by pressing `Ctrl + C` in the terminal.