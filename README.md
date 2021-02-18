Project: Grad-CAM (https://arxiv.org/abs/1610.02391)

Author: Willis Sanchez-duPont

Email: wsanchezdupont@g.hmc.edu

This is a repository for my implementation of grad-CAM using PyTorch. In order to use the implementation, the user must create an instance of the Grad-CAM class with a model as input. Then when Grad-CAM is called on an input, the user must specify which submodule within the model will have its CAMs computed (typically the last layer of the feature extractor component). Please see the code for more info.

To test guided grad-CAM on the default image included in the repository, run the following command:

```python GradCAM.py --classes 243 281 --guided```

Additionally include the ```--device cuda``` option to enable GPU computation.

Dependencies (what I have downloaded - probably works with some earlier versions):

pytorch 1.4

numpy 1.16.5

opencv-python 4.1.2.30
