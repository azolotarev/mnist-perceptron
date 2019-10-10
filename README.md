Usage
- Google Colab

Dataset
- MNIST %url_to_mnist%

Framework
- PyTorch

Model architecture
- Simple fully connected network with 1 hidder layer
- Total parameters: 1000
- Hidden layer activation: ReLU
- Output layer activation: log softmax

Model training
- Loss: cross entropy 
- Optimizer: Adam
- 20 epochs with lr=1e-4 (0.001)
- 20 epochs with lr=1e-6 (0.00001)

Model evaluation
- correctly labeled / total images in the test set
