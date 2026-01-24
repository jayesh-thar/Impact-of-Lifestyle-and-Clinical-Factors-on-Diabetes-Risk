# Impact-of-Lifestyle-and-Clinical-Factors-on-Diabetes-Risk

## Here are the neccessary access points for our inventory
* Drive:
```bash
https://drive.google.com/drive/folders/1m9yJzzcswyZwosk_CMy8a0hJuivnnHa9?usp=sharing
```
* Repo :
```bash
https://github.com/jayesh-thar/Impact-of-Lifestyle-and-Clinical-Factors-on-Diabetes-Risk
```
---
### Upload the dataset from kaggle to goolge colab directly
* Step 1: Make the kaggle.json file from the kaggle and upload it to the colab before going to step 2
  ``` ruby
  {"username": "USER_NAME", "key": "API_KEY"]
  ```

* Step 2: 
``` bash
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/

!kaggle datasets download -d iammustafatz/diabetes-prediction-dataset

import zipfile
zip = zipfile.ZipFile("/content/diabetes-prediction-dataset.zip",'r')
zip.extractall("/content")
zip.close()
```

* Step 3:
```bash
import pandas as pd
df = pd.read_csv("/content/diabetes_prediction_dataset.csv")
df.head()
```
