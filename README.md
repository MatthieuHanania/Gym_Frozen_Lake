# Gym_Frozen_Lake
I train an agent on the gym frozen lake environment 

![](https://www.gymlibrary.dev/_images/frozen_lake.gif)

The environment description is available here : https://www.gymlibrary.dev/environments/toy_text/frozen_lake/


There are 2 properties of the env.
 - Slippery model: at each movement, the agent has a certain probability to slip and to move on another case
 - Non slippery model: the agent moves normally. 


The objective is to train reinforcement learning model. So the environment defines rewards:
- Reach goal(G): +1
- Reach hole(H): 0
- Reach frozen(F): 0

For each episode, if the agent falls or get the goal , it restarts

 
 __The slippery model need more training to obtain a good score__
 
####### Tensorboard #######

This graph represents the model score,
I train it 10 times on 1e4 episodes. Each training is represented by a color, and the gray curve represent the global training.

<img src="https://github.com/MatthieuHanania/Gym_Frozen_Lake/blob/main/non%20slippery%20agent%20mean%20episode%20lenght.png" width="500">
 
 
 __The non slippery model is more efficient__
 
 ####### Tensorboard #######
 
 Compared to the slippery model, the non slippery, does not need a lot of trains to succeed. 
 And the more we train it, the faster it is (less episode length), and it also has a better score.
 
 <img src="https://github.com/MatthieuHanania/Gym_Frozen_Lake/blob/main/non%20slippery%20agent%20score.png" width="500">
 
 <img src="https://github.com/MatthieuHanania/Gym_Frozen_Lake/blob/main/non%20slippery%20agent%20mean%20episode%20lenght.png" width="500">
