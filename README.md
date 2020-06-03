# Training ML-Agents on Google Colab

<h4 align="center">
    For training Unity's built environment with ML-Agents on Google Colaboratory
</h4>

## What’s In This Document
- [Introduction](#introduction)
- [Prerequisites Tools](#prerequisites-tools)
- [Setup Instructions](#setup-instructions)
- [License](#license)


## Introduction

After struggling, on a particular question (**How to run ML-Agents on Google Colab?**) for days I thought it would be great to create a github repo to share my findings on this topic (after solving this question) as there is little to no information on the internet. This repo gives information on the above question by testing an example environment on colab. (This example environment is taken from ML-Agents repo)

The environment is built using server/headless mode in Unity. So when I was working on Reinforcement Learning with Ml-Agents (an interface provided by Unity which is used to communicate with the learning environment made using Unity game engine). I felt the need to have one more pc because training requires hours to get completed and it almost used my RAM to its full potential. So I decided to shift the training process on google colab. And here I am gonna tell how I did this. 

## Prerequisites Tools

- **Unity Game Engine :**
It is used to create, modify, and build the training environment in server/headless mode for the Linux system. Get the latest version of this software [here](https://unity3d.com/get-unity/download/archive).


## Setup Instructions

Run [**this**](./ML_Agents-with-Colab.ipynb) python notebook on Google Colab. This will clone the release_1 branch from ML-Agents github repo to colab. For the next step, it will clone this repo to get the example environment and provides the appropriate permissions to the Linux executable i.e. (.x86_64). And after this, it will enable the tensorboard and start the training process.

In the end, you can download the .nn file for the /content/models/${run_id} folder to embed that in your Unity environment for the inference process.


## License
Licensed under the [MIT License](./LICENSE).
