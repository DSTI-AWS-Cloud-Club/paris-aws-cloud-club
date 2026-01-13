# Phase 1 - Deploy an artifact in the cloud
Integrate a ML artifact into S3 and using Lambda call through an API

## Steps

Clone the repository

```
uv init

uv python install 3.11

uv python pin 3.11

uv add ---


```

Activate environment

On Windows:
`.\.venv\Scripts\activate.ps1`  

On Linux:

`source .venv/bin/activate`


## The AWS services involved

- **S3 Integration**: Data and model storage in `housing-regression-data` bucket
- ** Lambda ** :  Functions that can run a python script
- **API Gateway**: REST API endpoint service


