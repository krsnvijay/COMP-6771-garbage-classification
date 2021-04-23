```
conda create -n garbage-classifier python=3.8 numpy scipy pandas tqdm opencv scikit-learn pip ipykernel pytorch torchvision cudatoolkit=10.2 -c pytorch
```

```
python -m ipykernel install --user --name garbage-classifier --display-name "garbage-classifier"
```
