# ars
 
Augmented Random Search is truly one of the most mindblowing algorithms I’ve come across with my research in reinforcement learning.

Augmented Random Search(ARS) is actually up to 15 TIMES FASTER than other algorithms with higher rewards in specific applications! That’s insane!

One of the ways, ARS is able to be so much faster is that unlike a lot of reinforcement learning algorithms that use deep learning with many hidden layers, augmented random search uses perceptrons! There are fewer weights to adjust and learn, but at the same time, ARS manages to get higher rewards in specific applications!

# Method of Finite Differences
The goal of reinforcement learning is to get an agent to learn something and similar to how deep reinforcement learning algorithms use gradient descent to optimize weights and reduce the cost function, ARS uses the method of finite differences to adjust its weights and learn how to perform a task.

# The Process
To update the weights effectively, the agent takes a random matrix of tiny values and adds them to the weights. The AI then adds the exact same matrix, but these same values, but this time with negative weights. It then repeats this many times and the end result is an agent trying to perform a task with slightly different weights.

We get rewards for each configuration of weights from the environment and some are higher than others. What ARS does it that it adjusts those weights according to the weight configurations that it gave the best rewards. The higher the reward, the more the weights were adjusted, the lower the reward, the lesser the weights were adjusted.

ARS also does things a little bit differently than other algorithms by exploring policy spaces instead of action spaces. Basically, this means that instead of analyzing the rewards it gets after each action, it analyzes the reward after a series of actions to determine if that set of actions led to a higher reward.

To sum up the main ideas:
- ARS uses a perceptron instead of a deep neural network.
- ARS randomly adds tiny values to the weights along with the negative of that value to figure out if they help the agent get a bigger reward.
- The bigger the reward from a specific weight configuration, the bigger its influence on the adjustment of the weights.

The test result, video result and research paper is attached with this repo.
