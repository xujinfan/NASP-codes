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

## Reference
```
@techreport{yao2019differentiable,
  title = {Differentiable Neural Architecture Search via Proximal Iterations},
  author = {Yao, Quanming and Xu, Ju and Tu, Wei-Wei and Zhu, Zhanxing},
  institution = {arXiv preprint arXiv:1905.13577},
  year = {2019}
}

@TechReport{quanming2018auto,
  author      = {Yao , Q. and Wang, M.},
  title       = {Taking human out of learning applications: A survey on automated machine learning},
  institution = {Arxiv: 1810.13306},
  year        = {2018},
}
```

## Acknowledgement
The codes of this paper are based on the codes of DARTS (https://github.com/quark0/darts). We appreciate DARTS's codes and thank the authors of DARTS.
