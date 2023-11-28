# SML Lab 2 - Swedish Wisper

## Performance Improvements

### Model
**Hyperparameter tuning:** The hyperparameters in the model that can be tuned are for instance `learning rate`, `batch size`, `epochs` and `warmup steps`. In the documentation it says that the `learning rate` is the "initial learning rate", so we are a little bit unsure whether tuning this parameter actually helps since there maybe already is some form of learning rate adaption incorporated in the training.

**Model architecture:** The pretrained model architecture can be changed from `small` to `medium` or `large`. The downside of this is that the training time will be longer and require more resources.

**Training/Evaluation:** In order to actually find the best performing model Cross-Validation can be performed as well. 

### Data
**Dataset:** The size and quality of the dataset can greatly determine the performance of the model. You can either use a larger dataset, or merge two datasets (with some preprocessing to unify the format of the data) to form a bigger one.r

**Preprocessing:** Audio filtering is something that can be done on both training and live data to enhance the clarity of the speaker, creating higher quality data for the model. Audio normalization can also be applied to make the volume of different audio clips more uniform.