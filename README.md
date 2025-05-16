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

The Python documentation is a good place to consult in case you run into obstacles. You can find it [here](https://docs.python.org/3/library/venv.html).

### Virtual environment for R

The R virtual environment is created using the `renv` package. Renv stores the dependencies in a renv.lock file. 

If you want to install the packages listed in the `renv.lock` file, you can run the following command:

```r
renv::restore()
```

Please consult the [renv documentation](https://rstudio.github.io/renv/articles/renv.html) for more information on how to use renv.