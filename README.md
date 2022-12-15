
# Neural Style Transfer

These python notebooks contain the code to run our experiments for neural style transfer

## Contributors
  - Zihao Deng (zihaoden@seas.upenn.edu)
  - Xuanmin Zhu (xuanminz@seas.upenn.edu)


# Code for running the experiments on Image style transfer

We have all the code for doing image style transfer and the corresponding experiments in the notebook ``neural_style_transfer.ipynb``

## Structure of the code framework
We have structured the code into sections, and the overall framework is shown below. Note that you do not need to install any packages and all of the libraries we have used are already installed in a default Colab environment. But you will need to connect to a GPU runtime in order for the code to work.

```
Imports and Preprocess
CNN Models
Style Loss
Content Loss
Model with Loss
  ├──VGG19
  ├──AlexNet
  ├──ResNet
Neural Style Transfer
Experiments
  ├──Image Evaluation Metric
  ├──Experiment: CNN Model
  |    ├──VGG19
  |    ├──AlexNet
  |    ├──ResNet
  ├──Experiment: Loss Function
  |    ├──L1 Loss
  |    ├──Smooth L1 Loss
  |    ├──Huber Loss
  |    ├──Restore MSE Content Loss
  ├──Experiment: Optimizer
       ├──Adam
       ├──SGD
       ├──Restore LBFGS optimizer
AMP
Generate Beautiful Image
```

You can easily run the code sequentially to reproduce all the results.
But you will need to upload your own images and make sure the file names matche strings in the notebook.
