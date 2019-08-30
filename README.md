# Differentiable Neural Architecture Search via Proximal Iterations
## Requirements
```
Python >= 3.5.5, PyTorch == 0.3.1, torchvision == 0.2.0
```
## Dataset
Prepare dataset firstly, dataset links can be seen in our Appendix. 

## Neural Architecture Search
python train_search.py

## Architecture Evaluation
python train.py --auxiliary --cutout # CIFAR-10
python train_tinyimagenet.py --auxiliary            # Tiny ImageNet

## Architecture Test
python test.py --auxiliary --model_path cifar10_model.pt # CIFAR-10
python test_tinyimagenet.py --auxiliary --model_path imagenet_model.pt # Tiny Imagenet

## Acknowledgement
The codes of this paper are based on the codes of DARTS (https://github.com/quark0/darts). We appreciate DARTS's codes and thank the authors of DARTS.
