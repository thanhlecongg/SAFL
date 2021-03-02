# SAFL: A Self-Attention Scene Text Recognizer with Focal Loss

This repository contains source code of research paper "SAFL: A Self-Attention Scene Text Recognizer with Focal Loss", which is accepted as full-paper in 19th Internation Conference on Machine Learning and Applications. Tested on seven scene text recognition benchmarks including: IIIT5K, SVT, ICDAR03, ICDAR13, ICDAR15, SVT-P and CUTE.

## Installation

```
conda env create -f environment.yml
conda install pytorch==1.2.0 torchvision==0.4.0 cudatoolkit=10.0 -c pytorch
```

## Train

```
bash scripts/stn_att_rec.sh
```

## Test

You can test with .lmdb files by
```
bash scripts/main_test_all.sh
```
Or test with single image by
```
bash scripts/main_test_image.sh
```

## Data preparation

We give an example to construct your own datasets. Details please refer to `tools/create_svtp_lmdb.py`.

## Citation

If you find this project helpful for your research, please cite the following papers:
