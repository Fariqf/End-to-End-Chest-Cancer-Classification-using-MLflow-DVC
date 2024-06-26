# End-to-End-Chest-Cancer-Classification-using-MLflow-DVC

## Workflows
1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the dvc.yaml

### dagshub
[dagshub](https://dagshub.com/)

MLFLOW_TRACKING_URI=https://dagshub.com/Fariqf/End-to-End-Chest-Cancer-Classification-using-MLflow-DVC.mlflow \
MLFLOW_TRACKING_USERNAME=Fariqf \
MLFLOW_TRACKING_PASSWORD=f25f49136f3dacf02762aa371cc1e52be10ac830 \
python script.py

Run this to export as env variables:

```bash

set os.environ["MLFLOW_TRACKING_URI"]="https://dagshub.com/Fariqf/End-to-End-Chest-Cancer-Classification-using-MLflow-DVC.mlflow"

set os.environ["MLFLOW_TRACKING_USERNAME"]="Fariqf"

set os.environ["MLFLOW_TRACKING_PASSWORD"]="f25f49136f3dacf02762aa371cc1e52be10ac830"
```

## To run dvc
1. Check .git in the working folder
2. command - 
``` bash
dvc init
dvc repro
dvc dag
```
3. dvc init will intialize the dvc folder
4. dvc repro will run the pipeline with given all artifacts and path
5. Run the file with dvc repro
6. dvc dag used to visualize the pipeline