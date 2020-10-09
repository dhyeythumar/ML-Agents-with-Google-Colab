# Training ML-Agents on Google Colab

<h4 align="center">
    For training Unity's built environment in server/headless mode with <a href="https://github.com/Unity-Technologies/ml-agents">ML-Agents</a> on Google Colaboratory.
</h4>


### Updates to my current project
Check out this [**youtube video**](https://youtu.be/4vwZNTagHsQ) on "<ins>Navigation strategies learned by an ML-Agent</ins>" on a custom environment made with Unity Engine.

And I'm also currently working on this environment to increase the difficulty level. *So, if anyone have suggestions/recommendations, feel free connect with me [here](mailto:dhyeythumar@gmail.com)*.


> **Important details about this repository:**
> - Unity engine version used to build the environment = 2019.3.15f1 (Different versions will work but make sure that you don't get errors while generating the binaries)
> - ML-Agents branch = release_1
> - Environment name = 3dball (sample environment provided in ML-Agents repo) (Upload all the files )
>
> **Environment in this repo is build for Linux with server/headless mode enabled with the help Unity engine.**
>
> **Upload all the files which are generated for the environment binary. Check out [this link](./headless_build/3DBall_example) to get an idea.**

## What’s In This Document
- [Introduction](#introduction)
- [Prerequisites Tools](#prerequisites-tools)
- [Setup Instructions](#setup-instructions)
- [Extra Information](#extra-information)
- [License](#license)


## Introduction

After struggling, on a particular question (**How to run ML-Agents on Google Colab?**) for days I thought it would be great to create a github repo to share my findings on this topic (after solving this question) as there is little to no information on the internet. This repo gives information on the above question by testing an example environment on colab. (This example environment is taken from ML-Agents [**repo**](https://github.com/Unity-Technologies/ml-agents))

So when I was working on Reinforcement Learning with ML-Agents (an interface provided by Unity which is used to communicate with the learning environment made using the Unity engine). I felt the need to have one more PC because training requires hours to get completed and also using my RAM to its full potential (until it is exhausted 🙁). So I decided to shift the training process on Google Colab. And here I am gonna tell how I did this. 

## Prerequisites Tools

- **Unity Game Engine :**
It is used to create, modify, and build the training environment in server/headless mode for the Linux system. Get the latest version of this software [here](https://unity3d.com/get-unity/download/archive).


## Setup Instructions

Run [**this**](./ML_Agents-with-Colab.ipynb) python notebook on Google Colab. This will clone the release_1 branch from ML-Agents github repo to colab. For the next step, it will clone this repo to get the example environment and provides the appropriate permissions to the Linux executable i.e. (.x86_64). And after this, it will enable the tensorboard and start the training process.

In the end, you can download the .nn file from the /content/models/${run_id} folder to embed that in your Unity environment for the inference process.


## Extra Information

The above-mentioned notebook only gives the trained (.nn) file and no visual observation while training, which I personally think has no fun at all. So after hunting down this question on the internet (i.e How to live stream the training process on twitch platform while the agents are learning?) so I can observer and find any errors or new behavior in agents. So if you are interested then keep reading or else you are good to go with the above settings.

So check out this [youtube video](https://youtu.be/dLMkE8R5nTA) as an example that I have trained on google colab and live-streamed the whole training visuals to twitch and then export to youtube (because twitch only saves the video for 14 days). This process is done in a different notebook and it requires different settings for the environment build file. (The example environment used for this process is also given in ML-Agents [**repo**](https://github.com/Unity-Technologies/ml-agents))


## License
Licensed under the [MIT License](./LICENSE).
