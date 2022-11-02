# README
The PyTorch implementation for RAM

## Environments

- Python 3.7.11
- PyTorch (version: 1.10.2)
- Numpy (version: 1.21.2)

## Dataset

We include the six processed datasets in the "data" folder.

## Example
Please refer to the following example on how to train and evaluate RAM on ML-1M

Please change the value of "dataset", and the hyper parameters (e.g., maxlen for $n$) as presented in our manuscript to reproduce the results on the other datasets.

You are recommended to run the code using GPUs.

RAM:

```
python main.py --dataset=ml1m --train_dir=default --maxlen=200 --hidden_units=512 --num_heads=4 --num_blocks=4 --num_epochs=301 --isTrain=0 --model=RAM
```

## Acknowledgement

The implementation is primarily built on [SASRec](https://github.com/pmixer/SASRec.pytorch). Thanks for the great work!