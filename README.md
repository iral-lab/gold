# GoLD

[Arxiv paper](https://arxiv.org/pdf/2007.14987.pdf)

Patrick Jenkins<sup>1</sup>, Rishabh Sachdeva<sup>1</sup>, Gaoussou Youssouf Kebe<sup>1</sup>, 
Padraig Higgins<sup>1</sup>, Kasra Darvish<sup>1</sup>, Edward Raff<sup>1, 2</sup>,
Don Engel<sup>1</sup>, John Winder<sup>1, 3</sup>, Francis Ferraro<sup>1</sup>, Cynthia Matuszek<sup>1</sup>

<sup>1</sup> <sub>University of Maryland, Baltimore County (UMBC)</sub>  
<sup>2</sup> <sub>Booz Allen Hamilton</sub>
<sup>3</sup> <sub>Johns Hopkins Applied Physics Laboratory</sub>

## Table of contents 

* [1. Introduction](#1-introduction)
* [2. Dataset downloading](#2-dataset-downloading)
* [3. How to cite](#3-how-to-cite)

## 1. Introduction

The **G**r**o**unded **L**anguage **D**ataset, or GoLD, is a grounded language learning dataset in five modalities: RGB, depth, text, transcribed speech, and speech. The data contains 207 instances of 47 object classes. The objects are from five high level categories of _food_, _home_, _medical_, _office_, and _tool_. Each instance is captured from different angles for a total of 825 images. Text and speech descriptions are collected using Amazon Mechanical Turk (AMT) for a total of 8250 text descriptions and 4059 speech descriptions.

The data is intended for use in multimodal grounded language acquisition tasks for domestic robots and for testing algorithmic differences between the domains.

## 2. Dataset downloading

The dataset consists of a directory of images, a directory of wav files, and two tsv files with descriptions. Each image label is formated as \<object name\>\_\<instance number\>\_\<frame number\>. wav files are labeled as \<object name\>\_\<instance number\>\_\<frame number\>\_\<description number\>.

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

[speech.tsv](speech.tsv) contains 6 fields
- hit_id: AMT hit id
- worker_id: anonymized worker id
- worktime_s: time in seconds to complete the AMT task
- item_id: label for the object, instance, and frame number
- wav: name of the related wav file in the speech directory
- transcription: the Google speech-to-text transcription

[text.tsv](text.tsv) contains 5 fields:
- hit_id: AMT hit id
- worker_id: anonymized worker id
- worktime_s: time in seconds to complete the AMT task
- item_id: label for the object, instance, and frame number
- text: a single text description for this instance

Video files are available upon request.

## 3. How to cite

```
TODO: bibtex
```
