# Adversarial Attacks on Object Detection in Optical Remote Sensing Images: Benchmarks

To facilitate the evaluation of the following research regarding adversarial attacks on object detection in O-RSIs, we sample 2000 images from the testing subset of [DIOR](https://gcheng-nwpu.github.io/#Datasets) and the validation subset of [DOTA](https://captain-whu.github.io/DOTA/index.html), respectively, dubbed DIOR-A and DOTA-A. The class-wise instance distributions of them are exhibited below. Here, both the class-wise instance distribution histograms and their corresponding Kernel Density Estimation (KDE) curves are plotted. These datasets are firstly leveraged in [Threatening Patch Attacks on Object Detection in Optical Remote Sensing Images](https://arxiv.org/abs/2302.06060) for the evaluations. For the training details of the victim detectors, we refer our users [TPA](https://github.com/plpl2019/TPA) for more detailed descriptions.

<img src="dist.png" alt="Class-Wise Instance Distributions." align=center />

## Architecture
These datasets are zipped in ./datasets.zip, where the architecture of this file is:
```
.datasets
├── DIOR-A
      ├──images
      └──labelTxt
└── DOTA-A
      ├──images
      └──labelTxt
```
Here, the image file and the coresponding label file are named with the same series number, e.g., 

An image file with the file name of ```./datasets/DIOR-A/images/11726.png```,

then its label file is ```./datasets/DIOR-A/labelTxt/11726.txt```


## Acknowledgement
We sincerely thank the authors of [DIOR](https://gcheng-nwpu.github.io/#Datasets) and [DOTA](https://captain-whu.github.io/DOTA/index.html) for their great contributions to optical remote sensing images understanding.


## Citation
If you use these datasets, please cite the following:
```
@article{sun2023threatening,
  title={Threatening Patch Attacks on Object Detection in Optical Remote Sensing Images},
  author={Sun, Xuxiang and Cheng, Gong and Pei, Lei and Li, Hongda and Han, Junwei},
  journal={arXiv preprint arXiv:2302.06060},
  year={2023}
}
```

