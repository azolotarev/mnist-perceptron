Usage

You have two options:
1. Run it locally on your machine, or
2. Run it with Google Colab

Running it locally
You'll need Jupyter Notebook or Jupyter Lab installed and GPU with CUDA support.
1. Download the repository as ZIP, or
2. git clone https://github.com/azolotarev/mnist-perceptron.git

Run PyTorch_MNIST_Perceptron.ipynb with Jupyter
Don't forget to uncomment !wget lines to download the dataset. You can comment them after.


Running it with Google Colab
1. Go to https://colab.research.google.com
2. File - Open notebook... (or press ctrl + o)
3. Select 'GITHUB'
4. 'Enter a GitHub URL...', paste this: azolotarev/mnist-perceptron
5. Select PyTorch_MNIST_Perceptron.ipynb
6. After the notebook has loaded, uncomment !wget lines
7. Change the runtime type to GPU: Runtime -> change runtime type -> hardware accelerator
8. press ctrl+f9 to run all cells.

Dependencies
- PyTorch-1.2.0 - main deep learning framework with awesome flow control
- idx2numpy-1.2.2 - to unpack the dataset directly into numpy arrays
- numpy - numerical computation
- gzip - unpacking .gz archives
- matplotlib - plotting library


Dataset
- MNIST http://yann.lecun.com/exdb/mnist/

DL Framework
- PyTorch GPU

Model architecture
- Simple fully connected network with 1 hidder layer
- Total parameters: ~1000
- Hidden layer activation: ReLU
- Output layer activation: log softmax

Model training
- Loss: cross entropy
- Optimizer: Adam
- 20 epochs with lr=1e-4 (0.001)
- 20 epochs with lr=1e-6 (0.00001)

Model evaluation
- TODO: add this
