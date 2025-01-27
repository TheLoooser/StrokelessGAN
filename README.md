# StrokelessGAN
**Note**: The current software works well with PyTorch 1.4.


If you use this code for your research, please cite:






## Prerequisites
- Linux or macOS
- Python 3
- CPU or NVIDIA GPU + CUDA CuDNN

## Getting Started
### Installation

- Clone this repo:
```bash
git clone https://github.com/JinshanZeng/StrokeGAN
cd StrokeGAN
```

- Install [PyTorch](http://pytorch.org) and 0.4+ and other dependencies (e.g., torchvision, [visdom](https://github.com/facebookresearch/visdom) and [dominate](https://github.com/Knio/dominate)).
  - For pip users, please type the command `pip install -r requirements.txt`.
  - For Conda users, you can create a new Conda environment using `conda env create -f environment.yml`.


###  train/test

- To view training results and loss plots, run `python -m visdom.server` and click the URL http://localhost:8097.
- Train a model:
```bash
#train
python train.py --dataroot ./data --name data_cyclegan --model cycle_gan
```

- Test the model:
```bash
#!./scripts/test_cyclegan.sh
python test.py --dataroot .data --name data_cyclegan --model cycle_gan
```



## [Datasets](docs/datasets.md)
https://github.com/JinshanZeng/Stroke_Based_Chinese_Character_Generation_Dataset

## [Training/Test Tips](docs/tips.md)
Best practice for training and testing your models.

## [Frequently Asked Questions](docs/qa.md)
Before you post a new question, please first look at the above Q & A and existing GitHub issues.


## Citation
If you use this code for your research, please cite our papers.
```
https://arxiv.org/abs/2012.08687
```


## Related Projects
**[CycleGAN-Torch](https://github.com/junyanz/CycleGAN) 
**[CycleGAN and pix2pix in PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)



## Acknowledgments
Our code is inspired by [pytorch--CycleGAN-and-pix2pix](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
