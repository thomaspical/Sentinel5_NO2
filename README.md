Sentinel5_NO2 V2
==============================

Downloading, cleaning and aggregation of NO2 (Nitrogen Dioxide) datas from the European satellite Sentinel5. This work is being carried out as part of the AMSECovid19 project.

DOWNLOAD AVAILABLE HERE : https://drive.google.com/drive/folders/1fJWwxo8MXBL7DKDqvwYQVlYa2W7g0TpQ?usp=sharing

MAJOR UPDATE : Complete overhaul of the file structure. Addition of a powerful logging system and a progressbar. Optimization of the code. 

Increase of ~30-50% in file size and processing time, with the benefit of less RAM required and new information essential for data processing: 
Wind angle, surface altitude, number of observations, snow/ice flag, soil classification, quality decreased to > 0.5, surface pressure...

Change of the data source: ONDA DIAS imposed a restrictive archiving system. We now use CREODIAS. 


Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    │
    ├── datas_sentinel5    <- You have to look here if you are only interested in downloading the data.
    │   ├─ archives_old        <- Previous version of archived files
    │   ├─ archives            <- File in which the files are recorded and definitively processed
    │   ├─ cleaned             <- Folder where cleaned, non-aggregated records are temporarily stored.
    │   ├─ csv                 <- Data file extracted from the ONDA DIAS API to obtain the links to
    │   │                         download the files.
    │   └─ tracking_files.csv  <- Automatically generated file, allows you to record the days processed,
    │                             with the number of files downloaded. This makes it possible to detect
    │                             the presence of new files for a day that has already been downloaded.
    │
    ├── get_sentinel5_V2.ipynb <- Notebook to get datas. Not available.
    │
    └── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
                              generated with `pip freeze > requirements.txt`

--------
