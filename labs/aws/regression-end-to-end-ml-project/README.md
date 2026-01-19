# Regression End to End ML project
This project uses a House TS Data set to create a regression model.

We are going through the steps from loading and treating the data to deploy and serve the model into the cloud.

This lab is inspired on the great work made by [Anas Riad](https://github.com/anesriad/Regression_ML_EndtoEnd).

The codebase is organized into distinct pipelines following the flow:
`Load → Preprocess → Feature Engineering → Train → Tune → Evaluate → Inference → Batch → Serve`

Here a description of the steps of our end-to-end pipeline:

- **Preprocessing**: Data Split / Data Cleaning / Data quality check (*Great expectations*)
- **Feature Engineering**: Transform features / Encoding / tests
- **Train, Tune, Evaluation & Model Tracking**: Model optimization (*Optuna* for hyper parameter tuning), Performance metrics and model tracking (*MLFlow* for experience tracking)
- **Set pipelines**: Feature, training and inference pipelines
- ** Containerize & CI / CD ** : Reproducibility (*Docker*), run, test and push to AWS (*Github Actions* to automate deployment)
- **Deploy & Serve** : Production API (*FastAPI* / *AWS ECS* )
- **Frontend**: Streamlit

## Project 
To ease understanding, since we could have different levels of knowledge between the members of the Club, we are going to divide the project increasing its complexity.  
The division is as follows:

1. *Phase1*: Integrate a ML artifact into S3 and using Lambda call through an API
2. *Phase2*: Code our ML pipeline into an application and integrate it in an EC2 instance.
3. *Phase3*: Full integration (original Anas Riad project) -> Integrate the whole End to End pipeline.

## The AWS services involved

- **AWS S3 Integration**: Data and model storage in `housing-regression-data` bucket
- **Amazon ECR**: Container registry for Docker images
- **Amazon ECS**: Container orchestration with Fargate
- **Application Load Balancer**: Traffic distribution and routing
- **CI/CD Pipeline**: Automated deployment via GitHub Actions


## Pre-requisites
1. An IDE (VSCode, PyCharm) that has **Colab** extension installed
2. Make sure `uv` is installed in your computer. If not installed go [here](https://docs.astral.sh/uv/getting-started/installation/#__tabbed_1_1) and install it depending on your OS. 
    2.1. *To test it*: run `uv` in a terminal in your computer. 
          You should have a response starting with *"An extremely fast Python package manager..."*

3. 
4.

