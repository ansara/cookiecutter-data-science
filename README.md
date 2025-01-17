# Cookiecutter Data Science (@ansara)

This is my customized version of the DrivenData Data
Science [cookiecutter](http://drivendata.github.io/cookiecutter-data-science/).

It initializes a boilerplate repo for my ML and data engineering projects according to contemporary best practices and
my preferences. This is a WIP. Enjoy!

### Changelog (Updated May 2021):
-----------

- Add [DVC](https://github.com/iterative/dvc) data version control
- Add Makefile rule 'version_control' for version control initialization
- Set Python 3 venv module as default virtual environment
- Add Python 3.7, 3.8, and 3.9 interpreter specifications
- Remove Python 2 interpreter support
- Change generated repo name format from 'foo_bar' to 'foo-bar'
- Remove default MIT license
- Removed Conda Package Manager support

### Requirements:
-----------

- Python 3.6+
- [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0

``` bash
$ pip install cookiecutter
```

### To start a new project, run:
------------

    cookiecutter -c v1 https://github.com/ansara/cookiecutter-data-science

[![asciicast](https://asciinema.org/a/244658.svg)](https://asciinema.org/a/244658)

### New version of Cookiecutter Data Science
------------
Cookiecutter data science is moving to v2 soon, which will entail using the command `ccds ...` rather
than `cookiecutter ...`. The cookiecutter command will continue to work, and this version of the template will still be
available. To use the legacy template, you will need to explicitly use `-c v1` to select it. Please update any
scripts/automation you have to append the `-c v1` option (as above), which is available now.


### The resulting directory structure
------------

The directory structure of your new project looks like this:

```
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io
```

### Installing development requirements
------------

    pip install -r requirements.txt
