---
title: "Secure DL"
excerpt_separator: "Secure Deep Learning"
author: Shital Adhikari
sidebar:
    - title: "Shital"
---
# WIP: Securing Deep Learning Processes
## Why

The real world application of deep learning involves face detection, finger print detection, processing of sensitive documents like passports, and other personal documents. Sharing such information to the developer and also securing these critical digital information is sensitive and needs to be dealt with care. Majority of existing deep learning model does not take security into consideration. In order to secure such information, we need both data security and the model security. We can secure both data and model by encrypting the model. But it is not such straight forward to implement these both. 

Encryption is useful, only when we can train our model to learn the features which are similar to the non-encrypted images.Homographic Encryption method can be used to encrypt our image data, (:warning: **We can apply non-linear operation in HE. But Why:question:**).


In regard to the, model weights we can use the load the model in the user end and deploy it locally. But the learned features could be reversed engineered which might leak the sensitive information. Instead we can make the model weights encrypted. (**How:question:**)

## Different methods to secure deep learning process
1. Hardware level privacy aware deep learning
2. Federated learning for to deploy privacy aware module



## TODO
- [ ] Implementing the homomorphic encryption in images

## Resources
1. [Homomorphic Encryption Details](https://blog.openmined.org/build-an-homomorphic-encryption-scheme-from-scratch-with-python/#buildanhomomorphicencryptionscheme)


