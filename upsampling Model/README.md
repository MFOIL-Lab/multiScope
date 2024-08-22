This repository is an official PyTorch implementation of the paper **"A cortex-wide multimodal microscope for simultaneous Ca2+ and hemodynamic imaging in the awake mouse"**.

## Dependencies
* Python 3.8.5
* torch = 1.12.0
* numpy
* skimage
* matplotlib
* tqdm
* opencv-python

## Code
```bash
git clone https://github.com/MFOIL-Lab/multiScope
```

## Training
```bash
python main.py --template proposed_x2 --scale 2 --patch_select grad_window --loss 1*RL1 --batch_size 8 --gpu_ids 0
```

## Testing
```bash
python main.py --template proposed_x2 --scale 2 --patch_select grad_window --loss 1*RL1 --batch_size 8 --gpu_ids 0 --test_only
```

## Problem
This project code references EDSR.
Run error problem solution can refer to https://github.com/sanghyun-son/EDSR-PyTorch.git
