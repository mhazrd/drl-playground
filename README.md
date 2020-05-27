[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Deep RL Project: Navigation

## Introduction

The project's objective is to train an agent to navigate and obtain yellow bananas in the following Unity environment.

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and the codes in the notebook will train an agent to achieve an average score of +13 over 100 consecutive episodes by using DQN algorithm.


## Getting Started

#### Requirements
- Linux OS
- Python environment
- [Unity Banana environment](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Git

#### Steps

1. Install Git and Anaconda

2. Create Python environment on Anaconda
```
conda create --name drl python=3.6
conda activate drl
```

3. Clone the the following repository and install Python dependencies to run the code
```
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```

4. Create IPykernel to use the current environment
```
python -m ipykernel install --user --name drl --display-name "drl"
```

5. Download the following Linux Unity environment zip archive file.
    - [Unity Banana environment](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)  

6. Place the file in the current root folder of this repository, and unzip (or decompress) the file. 

7. Run Jupyter/Ipython Notebook and Change the kernel to "drl"

8. Make Unity Environment to point to the file decompressed by the step 5
```
env = UnityEnvironment(file_name="./Banana_Linux/Banana.x86_64")
```


## Instructions

All the codes (Model, Training and Simulation) are written in `Navigation.ipynb`. Please follow the notebook from top to bottom to create, train and test the agent.
It can be directly modified for any changes inside a notebook