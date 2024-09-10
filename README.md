# MDP REPRESENTATION

## AIM:
To represent a Markov Decision Process(MDP) problem in the following ways.

1.Text representation

2.Graphical representation

3.Python - Dictonary representation

## PROBLEM STATEMENT:
```
DEVELOPED BY : Marella Dharanesh
REF NO : 212222240062
```
### Problem Description
An agent needs to pick product B from a supermarket where there are three products A , B and C

### State Space
{Product A , Product B , Product C}

### Sample State
Product A

### Action Space
[Left , Right , Pick}

### Sample Action
Left

### Reward Function
+1 - when an agent move to the right side and pick product B
0 - Otherwise

### Stochastic Transition Probability
In a stochastic MDP, the transition probabilities determine the likelihood of moving from one state to another after taking a certain action.

Transition Probability:

From Product A (State 0):

Left (Action 0): 100% chance to remain in Product A.

Right (Action 1): 100% chance to remain in Product A.

From Product B (State 1):

Left (Action 0): 100% chance to move to Product A.

Right (Action 1): 70% chance to move to Product C with a reward of +1, 30% chance to remain in Product B with no reward.

From Product C (State 2):

Left (Action 0): 100% chance to remain in Product C.

Right (Action 1): 100% chance to remain in Product C.
### Graphical Representation

![graphical diagram ](https://github.com/user-attachments/assets/ef153350-21f8-4342-ac6d-a084ae72479c)


## PYTHON REPRESENTATION:
```python3
P = {
    0:{
        0: [(1.0,0,0.0,True)],
        1: [(1.0,0,0.0,True)]
    },
    1:{
        0: [(1.0,0,0.0,True)],
        1: [(1.0,2,1.0,True)]
    },
    2:{
        0: [(1.0,2,0.0,True)],
        1: [(1.0,2,0.0,True)]
    }
}
```
## OUTPUT:

![pic RL DHARANESH](https://github.com/user-attachments/assets/9ae15c88-790a-4e14-b348-ab9119b3347b)

## RESULT:
Thus, the agent learns to pick product B from products A, B, and C by repeatedly interacting with the environment, receiving feedback in the form of rewards
