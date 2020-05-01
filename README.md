
Sentinel5_NO2
==============================

Downloading, cleaning and aggregation of NO2 datas from the European satellite Sentinel5. This work is being carried out as part of the AMSECovid19 project.

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    │
    ├── datas_sentinel5    <- You have to look here if you are only interested in downloading the data.
    │   ├─ archives            <- File in which the files are recorded and definitively processed
    │   ├─ cleaned             <- Folder where cleaned, non-aggregated records are temporarily stored.
    │   ├─ csv                 <- Data file extracted from the ONDA DIAS API to obtain the links to     │      │   │                         download the files.
    │   └─ tracking_files.csv  <- Automatically generated file, allows you to record the days processed,       │                             with the number of files downloaded. This makes it possible to detect        │                             the presence of new files for a day that has already been downloaded.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── notebooks          <- Notebooks folders
    │   ├── confidential
    │   │    └──secrets.py        <- Secret script where ID and password are saved to connect to ONDA DIAS     │   │                            with following elements: user="<your_username"
    │   │                            password = "<your_password>"
    │   ├── get_sentinel5.ipynb   <- Script to download, clean and reduce in loops ALL NO2 files               │   │                            availables from ONDA DIAS
    │   └── work_sentinel5.ipynb  <- Script to read and analyse ALL the cleaned files availables
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org


--------

<p><small>Project based on the <a target="_blank" href="http://git.equancy.io/tools/cookiecutter-data-science-project/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
