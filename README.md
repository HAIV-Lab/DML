# Decoupling MaxLogit for Out-of-Distribution Detection

## Data

```
|--data
|--|--cifar-100-python
|--|--ood_test
|--|--|--svhn
|--|--|--places365
|--|--|--LSUN_R
|--|--|--LSUN_C
|--|--|--iSUN
|--|--|--dtd
```



## How to inference

```python
python test_DML+.py cifar100 

--MCF cifar100_wrn_Focal_NN_epoch_199.pt 

--MNC cifar100_wrn_Center_NN_epoch_199.pt
```



## Results

```
Files already downloaded and verified
loading models
loading models

Textures Detection
                                Ours
FPR95:                  41.87   +/- 0.64
AUROC:                  91.11   +/- 0.20
AUPR:                   97.87   +/- 0.05


SVHN Detection
                                Ours
FPR95:                  17.58   +/- 0.39
AUROC:                  97.21   +/- 0.08
AUPR:                   99.43   +/- 0.02


LSUN-C Detection
                                Ours
FPR95:                  17.48   +/- 0.26
AUROC:                  97.23   +/- 0.05
AUPR:                   99.42   +/- 0.01


LSUN-R Detection
                                Ours
FPR95:                  27.72   +/- 0.66
AUROC:                  94.51   +/- 0.15
AUPR:                   98.75   +/- 0.04


iSUN Detection
                                Ours
FPR95:                  29.89   +/- 1.06
AUROC:                  93.84   +/- 0.24
AUPR:                   98.58   +/- 0.06


Places365 Detection
                                Ours
FPR95:                  71.70   +/- 0.28
AUROC:                  82.45   +/- 0.48
AUPR:                   95.69   +/- 0.20


Mean Test Results
                                Our DML
FPR95:                  34.37
AUROC:                  92.72
AUPR:                   98.29

```

