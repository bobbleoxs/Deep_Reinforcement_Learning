##### **The Environment**

An agent navigates (and collects bananas) in a large, square world simulated in Unity engine. 

![banana_untrained](media/15891326885742/banana_untrained.gif)

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

`0` - move forward
`1` - move backward
`2` - turn left
`3` - turn right
    
The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

**Getting Started**

Download the environment from one of the links below. You need only select the environment that matches your operating system:


Linux: click [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
        Mac OSX: click [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
        Windows (32-bit): click [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
        Windows (64-bit): click [here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
(For Windows users) Check out this link if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not enabled a virtual screen), then please use this link to obtain the environment.

Place the file in this folder, unzip (or decompress) the file and then write the correct path in the argument for creating the environment under the notebook Navigation.ipynb:

`env = UnityEnvironment(file_name="Banana.app")
`

Then run the `Navigation.ipynb` notebook using the drlnd kernel. Hyper parameters are saved in the file `checkpoint_dqn.pth`.

