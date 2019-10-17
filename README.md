# TRAIit
## About:
“trAIn it” is a game concept in which it is integrated with an AI game bot where the user trains it in the game itself by playing with it. Which is later competed with the other game bot of other player. So the skills of the bot are directly proportional to the time user spends with his/her bot. This can be applied to a wide set of games.

## Our Game Plan:
To keep it simple, I initially am expecting it to use the idea on the ping pong game. Here the user is an Old wrecked bat which trains the new generation young bats (which is a bot) to play ping pong and send them to play with the other young bats of other users.

So, it is a ping pong game in which both the players are bots, where skills of either bots depends upon the type of learning algorithm it uses and the time it has been put through the training. Here training implies the training of the neural network by the user while actually playing with it. I have initially tried equipping the player bot with the deep Q learning neural network which seemed to take a lot of time to atleast make it play sensible. To counter this problem, instead of training it from the scratch while playing with it, I started it with an already trained model which is saved till some checkpoint using openAI's gym environment. Though it drastically decreased the time play for the user to train the game bot, it couldn't match the needed expectations to keep an user excited for the time he has to invest to see a change in the bot's performance. So I tried implementing the policy gradients method and saving models at different checkpoints and let user decide to train from what pre-trained level he can pick the bot from and train further. User, then can make his bot compete with other game bots which are trained by other users.
 

## Implementation results:


### 1. Ping Pong using Deep Q Learning:

After training the algorithm on the ping pong game environment for a week there was a change in the behavior of the Academic AI (on right side) when allowed to play with the Consumer AI (on left). Though the results were not inhabitable to my use case, there was improvement.

![](https://github.com/sannzay/TRAINit/blob/master/Images/t.1.png)


### 2. Ping Pong using Policy Gradient:

After training for almost 90 hours it achieved a notable result. The Academic AI beat Consumer AI by 5 scores when the total score to win an episode was 20. Green bat is the Academic AI which learns. Orange is Consumer AI which acts according to the heuristics it is designed with.

![](https://github.com/sannzay/TRAINit/blob/master/Images/t.2.jpg)



## Scope:
This idea can be used on all current major games, like if we take a game “Pokemon Go”, Ash trains the Pikachu by playing with it and send it to the battle field to fight with other Pokemons. 
Like-wise its span is large and can be used in all kinds of games like:
1.	Dragon fantasy games
2.	Fighting games
3.	Logic games like chess
4.	Kid games
