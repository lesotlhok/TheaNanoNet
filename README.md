# TheaNanoNet
 Lightweight Deep Learning for Real-time Polyp Identification and Segmentation in Colonoscopy:  The Nano-Net Approach
 
Various arguments used in the above syntax are explained below –

X – The data is passed as input and can have the value of NumPy array or Numpy arraylike, TensorFlow tensor value, dict mapping names of input or list of tensors. A numpy array is specified when we need to pass multiple inputs to the model. A tensor or tensor list is also used in the same scenario. In contrast, dict mapping is used for specifying the names of the inputs corresponding to the tensors or arrays provided if the model contains the inputs named ones.

Y – It is the value of the data that is targeted. Even this value can be a Numpy array, tensor, or list of tensors, but the condition is that the value should be consistent with the x parameter. So, for example, we cannot have tensor inputs and NumPy targets or vice versa.

Batch_size – It has the value set to either None or integer and is used to specify sample count per update of a gradient. When not specified, the default value is considered as 32. When the input data is going to create generators of data sets, there is no need to mention the batch size.

Epochs – It is an integer number where we specify the epochs we must carry out to train the model. Epoch consists of an iteration for x and y data that are mentioned.

Verbose – It can have the value of 0, 1, 2, or auto where one is for the progress, 0 for silent, and auto is the default value set to 1, 2 is the value that specifies one line to be considered per epoch or iteration.

Callbacks – It is the list of the instances of callbacks that are implemented during training.

Validation_split – It has the float value and can be either 1 or 0, which is the specification of a fraction of training data that will be used for validation.

Validation_data – It is the data that will be considered for the loss evaluation and metrics for the model.

Class_weight is the optional parameter for mapping dictionary indices of class with the corresponding float or weight values that are used further for calculating the loss function.

Steps_per_epoch – It helps in mentioning the count of the steps that need to be used while jumping from one epoch completion to the beginning of the new epoch. When not mentioned, the default value is treated as Null.
