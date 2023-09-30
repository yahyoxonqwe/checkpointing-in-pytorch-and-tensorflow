# checkpointing-in-pytorch-and-tensorflow
## checkpoint in [pytorch](https://pytorch.org/tutorials/recipes/recipes/saving_and_loading_a_general_checkpoint.html) 
To save multiple checkpoints, you must organize them in a dictionary and use torch.save() to serialize the dictionary. A common PyTorch convention is to save these checkpoints using the .tar file extension. To load the items, first initialize the model and optimizer, then load the dictionary locally using torch.load(). From here, you can easily access the saved items by simply querying the dictionary as you would expect.

In this recipe, we will explore how to save and load multiple checkpoints.

## checkpoint in [tensorflow](https://www.tensorflow.org/tutorials/keras/save_and_load)
The phrase "Saving a TensorFlow model" typically means one of two things:     Checkpoints or  SavedModel.
    
Checkpoints capture the exact value of all parameters (tf.Variable objects) used by a model. Checkpoints do not contain any description of the computation defined by the model and thus are typically only useful when source code that will use the saved parameter values is available.


# Installation
Clone the repository:
``` bash
git clone https://github.com/yahyoxonqwe/checkpointing-in-pytorch-and-tensorflow.git
```
Change into the project directory:
``` bash
cd checkpointing-in-pytorch-and-tensorflow
```
Install the required dependencies:
``` bash
pip install -r requirements.txt
```
