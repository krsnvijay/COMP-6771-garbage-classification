# COMP 6771 Image Processing Project

Classify images of garbage using Custom CNN, ResNet50, VGG-16

## Main Dependencies

- Pytorch
- TorchVision
- Pandas
- Scikit learn
- Numpy

## Folder Structure

```
./code/environment-gpu.yaml <-- gpu conda environment for our project
./code/environment-cpu.yaml <-- cpu conda environment for our project
./code/garbage_classifier.ipynb <-- primary notebook to run the deep learning models
./code/data/ <-- contains garbage dataset used in the project
```

## Setup

- create conda environment from `environment-gpu.yml` using

```
conda env create -f environment-gpu.yml
```

- you could also use this command to create the environment instead of the yml file

```
conda create -n garbage-classifier python=3.8 numpy scipy pandas tqdm opencv scikit-learn pip ipykernel pytorch torchvision cudatoolkit=10.2 -c pytorch
```

- activate your conda environment using

```
conda activate garbage-classifier
```

- If using a jupyter notebook, use this command to create this pykernel, later change your kernel to this on jupyter.

```
python -m ipykernel install --user --name garbage-classifier --display-name "garbage-classifier"
```

## Instructions

- `garbage_classifier.ipynb` is the main notebook to run
- GPU is required to train the model faster, but our code is GPU agnostic will also work with a cpu
- After training the models are saved locally you can load them to perform predictions

## Dataset

The garbage dataset was downloaded from https://www.kaggle.com/mostafaabla/garbage-classification
