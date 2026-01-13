# Phase 1 - Deploy an artifact in the cloud
Integrate a ML artifact into S3 and using Lambda call through an API

## Steps

### 0.Clone the repository
Create a folder in your local system and clone the repository:

` git clone https://github.com/zBotta/paris-aws-cloud-club.git`

### 1.Initialise python env
Open your IDE and open the cloned repo. Open a terminal and run:

```
uv sync
```

#### 1.1 Activate environment

On Windows:
`.\.venv\Scripts\activate.ps1`  

On Linux:

`source .venv/bin/activate`

### 2. Get the data
Open `phase 1\notebooks\00_download_data.ipynb`

When using the notebook for the first time, **choose a kernel** from the **top-right** of the notebook.

Run the notebook `phase 1\notebooks\00_download_data.ipynb`.

The following directories will be created / populated by the download step:

```
data/
├── processed/
│   ├── train_data.csv
│   ├── validation_data.csv
│   └── test_data.csv
└── models/
    └── (model files go here, e.g. trained-model.pkl)
```

### 3. 

## The AWS services involved

- **S3 Integration**: Data and model storage in `housing-regression-data` bucket
- ** Lambda ** :  Functions that can run a python script
- **API Gateway**: REST API endpoint service


