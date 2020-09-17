# GoLD

[Arxiv paper](https://arxiv.org/pdf/2007.14987.pdf)

Patrick Jenkins<sup>1</sup>, Rishabh Sachdeva<sup>1</sup>, Gaoussou Youssouf Kebe<sup>1</sup>, 
Padraig Higgins<sup>1</sup>, Kasra Darvish<sup>1</sup>, Edward Raff<sup>1, 2</sup>,
Don Engel<sup>1</sup>, John Winder<sup>1, 3</sup>, Francis Ferraro<sup>1</sup>, Cynthia Matuszek<sup>1</sup>

<sup>1</sup> <sub>University of Maryland, Baltimore County (UMBC)</sub>  
<sup>2</sup> <sub>Booz Allen Hamilton</sub>
<sup>3</sup> <sub>Johns Hopkins Applied Physics Laboratory</sub>

The **G**r**o**unded **L**anguage **D**ataset, or GoLD, is a grounded language learning dataset in five modalities: RGB, depth, text, transcribed speech, and speech.

## Table of contents 

* [1. Introduction](#1-introduction)
* [2. Dataset downloading](#2-dataset-downloading)
* [3. How to cite](#3-how-to-cite)

## 1. Introduction

## 2. Dataset downloading

The structure of the image files looks like
```
images
└── color
    └── allen_wrench
        └── allen_wrench_1
            ├── allen_wrench_1_1.png
            ├── allen_wrench_1_2.png
            └── ...
        └── allen_wrench_2
            ├── allen_wrench_2_1.png
            ├── allen_wrench_2_2.png
            └── ...
        └── ...
    └── apple
        └── apple_1
            ├── apple_1_1.png
            ├── apple_1_2.png
            └── ...
        └── ...
    └── ...
└── depth
    └── allen_wrench
        └── ...
    └── apple
        └── ...
    └── ...
└── image_raw
    └── allen_wrench
        └── ...
    └── apple
        └── ...
    └── ...
└── pcd
    └── allen_wrench
        └── allen_wrench_1
            ├── allen_wrench_1_1.pcd
            ├── allen_wrench_1_2.pcd
            └── ...
        └── allen_wrench_2
            ├── allen_wrench_2_1.pcd
            ├── allen_wrench_2_2.pcd
            └── ...
        └── ...
    └── apple
        └── apple_1
            ├── apple_1_1.pcd
            ├── apple_1_2.pcd
            └── ...
        └── ...
    └── ...
```

## 3. How to cite

```
TODO: bibtex
```
