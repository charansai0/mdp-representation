# MDP REPRESENTATION

## AIM:
The representation of real world scenario using Markov Decision Process by stating all the states,actions and environment with respective rewards.

## PROBLEM STATEMENT:
To develop a game which will promote to other level,when the agent complete its task correctly.
### Problem Description
If the agent unable to complete the given task,then there is no promotion to other level,when it reaches the final level,it will recieve a reward.

### State Space
{L1,L2,L3}--->{0,1,2}
### Sample State
L1--->{0}

### Action Space
Moving Left(1)

Stay in the same level(0)

### Sample Action
Stay in the same level(0)

### Reward Function
+1(When it reaches the goal state or final level)

### Graphical Representation
![WhatsApp Image 2024-03-01 at 11 28 36 PM](https://github.com/charansai0/mdp-representation/assets/94296221/01fe0484-5538-481b-ac35-a5b4c8a87f60)


## PYTHON REPRESENTATION:
~~~

P = {
    0:{
        0: [(0.55,0,0,True),(0.13,1,0,False)],
        1: [(0.13,1,0,False),(0.55,0,0,True)]
    },
    1:{
        0: [(0.55,1,0,False),(0.13,2,1,True)],
        1: [(0.13,2,1,True),(0.55,1,0,False)]
    },
    2:{
        0: [(0.55,2,1,True),(0.13,1,1,False)],
        1: [(0.13,1,1,False),(0.55,2,1,True)]
    }
}


~~~

## OUTPUT:
![image](https://github.com/charansai0/mdp-representation/assets/94296221/7e09d35a-aa50-4b86-85c1-9f9ea7e0bb3c)


## RESULT:
Therefore an MDP representation has been created for a real world scenario with all the states, actions and rewards.
