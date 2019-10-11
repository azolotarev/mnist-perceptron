The main .ipynb notebook was created and tested in [Google Colaboratory](https://colab.research.google.com/)

## **Usage**

There are two options:

**1. Running locally**

You'll need [Jupyter Notebook](https://jupyter.org/) or [Jupyter Lab](https://github.com/jupyterlab/jupyterlab) installed and a GPU with CUDA support.

1. Download the repository as ZIP or clone with git:
```
git clone https://github.com/azolotarev/mnist-perceptron.git
```
2. Open *PyTorch_MNIST_Perceptron.ipynb* with Jupyter;
3. Uncomment *!wget* lines to download the dataset. You can comment them after;
4. Run the notebook.

**2. Google Colab**
1. Go to [Google Colab](https://colab.research.google.com/);
2. *File* -> *Open notebook* (hotkey: *ctrl + o*);
3. Select *GITHUB*;
4. In *Enter a GitHub URL...* form paste *azolotarev/mnist-perceptron*;
5. Select *PyTorch_MNIST_Perceptron.ipynb*;
6. *Runtime* -> *change runtime type* -> *hardware accelerator* -> change from *None* to *GPU*;
7. Uncomment *!wget* lines to download the dataset. You can comment them after;
8. Press *ctrl+f9* to run all cells or run them one by one with *shift+enter*.


## **Dependencies**
- *PyTorch-1.2.0* - main deep learning framework with awesome flow control
- *idx2numpy-1.2.2* - to unpack the dataset directly into numpy arrays
- *numpy* - numerical computation
- *gzip* - unpacking .gz archives
- *matplotlib* - plotting library


## **Dataset**
- [MNIST](http://yann.lecun.com/exdb/mnist/)

## **Model architecture**
- Simple fully connected network with 1 hidder layer
- Total parameters: ~1000
- Hidden layer activation: ReLU
- Output layer activation: log softmax

**Model training**
- Loss: cross entropy
- Optimizer: Adam
- 20 epochs with lr=1e-4 (0.001)
- 20 epochs with lr=1e-6 (0.00001)

## **Model evaluation**

I've chosen a simple accuracy metric to evaluate the model performance:

 *c ÷ t*
 
*c* - number of correctly labeled digits;
*t* - total number of digits in test dataset

Example: 946 correctly labeled images with a total of 1000 images in the dataset will result in 94,6% accuracy
