## The project Machine Learning CLassiFication (MLclf) 
### The project is to transform the mini-imagenet dataset which is initially created for the few-shot learning (other dataset will come soon...) to the format that fit the classification task.

### The transformed dataset is divided into train, validation and test dataset, each dataset of which includes 100 classes.

##

##### How to use this package:

```python
from MLclf import MLclf
# Download the original mini-imagenet data:
MLclf.miniimagenet_download(Download=True)
# transform the original data into the format that fits the task for classification.
train_dataset, validation_dataset, test_dataset = MLclf.miniimagenet_clf_dataset(ratio_train=0.6, ratio_val=0.2, seed_value=None, shuffle=True, save_clf_data=True)
```