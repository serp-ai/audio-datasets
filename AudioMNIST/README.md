## Interpreting and Explaining Deep Neural Networks for Classification of Audio Signals

![image](../assets/AudioMNIST.png)

**Image credit:**    [Christian Lillelund](https://www.kaggle.com/christianlillelund) on [Kaggle](https://www.kaggle.com/)

Deep neural networks have been successfully applied to problems in many domains. Understanding their inner workings with respect to feature selection and decision making, however, remains challenging and thus trained models are often regarded as black boxes. Layerwise Relevance Propagation (LRP) addresses this issue by finding those features that a model relies on, offering deeper understanding and interpretation of trained networks. This repository contains code and data used in **Interpreting and Explaining Deep Neural Networks for Classification of Audio Signals** (https://arxiv.org/abs/1807.03418).

### Repository structure

#### data (audioMNIST)
* The dataset consists of 30000 audio samples of spoken digits (0-9) of 60 different speakers. 
* There is one directory per speaker holding the audio recordings. 
* Additionally "audioMNIST_meta.txt" provides meta information such as gender or age of each speaker.

#### models
* There are two different model architectures and training parameters in the CAFFE deep learning framework format.
* Bash script to train and test models.

#### recording_scripts
* Scripts to gather further audio samples. 

#### preprocessing_data.py
* A python script to preprocess the provided audio records and to store them in a format suitable for the provided caffe models.


### Reference
If you use the provided audioMNIST dataset for your project, please cite [our paper](https://arxiv.org/abs/1807.03418):

```
@ARTICLE{becker2018interpreting,
  author    = {Becker, S\"oren and Ackermann, Marcel and Lapuschkin, Sebastian and M\"uller, Klaus-Robert and Samek, Wojciech},
  title     = {Interpreting and Explaining Deep Neural Networks for Classification of Audio Signals},
  journal   = {CoRR},
  volume    = {abs/1807.03418},
  year      = {2018},
  archivePrefix = {arXiv},
  eprint    = {1807.03418},
}
```

---

**[Dataset DAGsHub Repository](https://dagshub.com/mert.bozkirr/AudioMNIST)**

This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)
