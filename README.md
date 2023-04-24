# Chorus Essential Biodiversity Variables
This repository contains Python scripts that allow creating a dataset of Essential Biodiversity Variables (EBV-ready dataset) for the class of species traits by combining two sources of data:

* Files generated by inference models of acoustic activity of anuran amphibians.
* Files of climatic variables (dataloggers and nearby weather stations). These data are read and harmonized according to the chosen locations and temporal range, and the result is saved in a NetCDF file.

## Requiriments

Python 3.10

```
matplotlib==3.6.2
netcdf4==1.6.2
numpy==1.22.4
openpyxl==3.0.10
pandas==1.5.2
pillow==9.3.0
scikit-learn==1.0.2
seaborn==0.12.2
xarray==2023.3.0
```

1. Install [Conda](https://docs.conda.io/projects/conda/en/stable/)

2. Clone this repository

```
git clone https://github.com/breyner-posso/chorus_ebvs/
```

3. Unzip the content of the folder 'sample_data'. Once unzipped, the directory structure should appear as follows:

```
sample_data
├── INCT2055
│   ├── datalogger
|       └── INCT20955_datalogger_20191220_20200429.xlsx
│   ├── model_predictions
│       └── INCT20955_inferences.csv
│   └── weather_station
│       └── INCT20955_wstation_A845_20191220_20200419.xlsx
└── metadata_workflow.xlsx
```
