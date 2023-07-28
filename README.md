# Reinforcement Learning

1. type of machine learning where an agent learns to make decisions by taking actions in an environment. The agent is rewarded or penalized (gets positive or negative reinforcement), based on the results of its actions. The aim is to maximize the cumulative reward over time.
2. RL is about sequential decision-making because the decisions (actions) taken by an agent affect the future state of the environment and subsequent decisions. 
3. RL is about sequential decision making, aiming to choose a series of actions that maximizes some reward
4. the reward or penalty is given by the environment.
5. The agent performs an action, and the environment responds with a new state and a reward (or penalty, if the reward is negative).
6. The reward function is a part of the environment and it determines how much reward the agent gets for each action in each state.
7. The aim is to maximize the cumulative reward - each action might have a short-term reward, but the agent is supposed to plan and execute actions that will result in the maximum cumulative reward over time.

![image](https://github.com/DrishtiShrrrma/coherexhuggingface-RL/assets/129742046/b401dddb-605d-46b0-9fce-a503d5f95f58)

# RL Framework

1. Agent: The entity that learns and makes decisions.
2. Environment: The world in which the agent operates.
3. State: A comprehensive representation of the condition of the environment. The state consists of all the necessary information needed to determine how the environment will respond to an action.
4. Observation: The agent's perception of the state, based on its sensory capabilities. While the state represents the entire environment, the agent may not be able to fully observe it. The information that the agent can perceive is referred to as an observation.
5. Action: A decision made by the agent that affects the state.
6. Reward: A signal received by the agent after each action, indicating how good or bad the action was.
7. Policy: A strategy used by the agent to decide which action to take based on its current observation.

![image](https://github.com/DrishtiShrrrma/deepmindxhuggingface-RL/assets/129742046/0fed8f16-29e2-4fdb-aa2c-2663aeb1ee0a)


# State

1. the state of the environment represents all the information necessary to determine how the environment will respond to any given action. It is the condition of the environment rather than the agent.

# State Vs Observation

1. A state is a complete description of the condition of the environment. In an MDP, the state is assumed to be fully observable and it encapsulates all relevant information from the past.
2. An observation, on the other hand, is the agent's perception of the state. In a partially observable environment, the observation may not contain all the information about the state.


# Reinforcement Learning Vs Supervised Learning

1. In supervised learning, an algorithm learns from a training dataset that contains input-output pairs, whereas in RL, an agent learns from interacting with an environment and receiving rewards or penalties.
2. Supervised learning requires labeled data, while RL does not require explicit labels.
3. RL is about sequential decision making, aiming to choose a series of actions that maximizes some reward, while supervised learning is about mapping inputs to outputs.
4. RL uses trial and error to learn optimal policies, whereas supervised learning uses existing labels to learn.
5. RL involves an environment, states, actions, and rewards, while supervised learning involves input data and corresponding labels.
6. **RL involves a reward system that guides learning, whereas supervised learning minimizes a loss function.**
7. RL is usually more suitable for decision-making tasks, while supervised learning is more suitable for classification or regression tasks.

![image](https://media.licdn.com/dms/image/D4D12AQElNK01s9WngA/article-inline_image-shrink_400_744/0/1655204443710?e=1694649600&v=beta&t=9F64KGmsyQ2TdnhHyyYpc6QSs2zxhu-YCOPuqnJThc8)

# Real-world Examples of RL

1. AlphaGo: Developed by DeepMind, AlphaGo used reinforcement learning to master the game of Go, a complex board game. It managed to defeat a world champion Go player, which was considered a major achievement in the field of AI.
2. OpenAI's Dota 2 bot: This bot used reinforcement learning to master the game of Dota 2, learning to play the game at a level beyond human capabilities.
3. DeepMind's Atari Games: DeepMind developed a RL algorithm that learned to play several Atari games to a superhuman level, directly from pixel input. 
4. Autonomous vehicles: RL is used in the decision-making process for self-driving cars.

![image](https://github.com/DrishtiShrrrma/coherexhuggingface-RL/assets/129742046/97aeaed1-f55c-4a49-9014-2766ae85ac1b)

# Online Vs Offline RL

1. **Alternative names of Online RL:** Interactive learning, Incremental learning, Continual learning, Real-time learning; **Alternative names of Offline RL:**  Batch learning, Static learning, Historical data learning.
2. Online RL - agents learns via interacting w envio, Offline RL - agent learns w the help of pre-recorded dataset
3. Online learning can continuously adapt to changes in the environment, while offline learning cannot.
4. Online RL is preferred over offline when we have to deal w a dynamic environment


![image](https://github.com/DrishtiShrrrma/coherexhuggingface-RL/assets/129742046/4a2288ce-4262-4066-aebe-28f345c04297)

![image](https://github.com/DrishtiShrrrma/coherexhuggingface-RL/assets/129742046/3e57f46d-823a-48d2-af34-7b842c228115)


# Advantages of Online RL

1. The model can adapt to changes in the environment in real-time.
2. It allows the model to learn from new data immediately as it becomes available.

# Disadvantages of Online RL

1. The model may overfit to recent data and forget older experiences.
2. It can be computationally expensive as it requires constant updating.

# Advantages of Offline RL

1. The model can be trained on a fixed dataset, which can be optimized in terms of resource usage.
2. It allows the model to learn from a large amount of data before making predictions.
3. Computaionally less expensive

# Disadvanatages of Offline RL

1. The model cannot adapt to changes in the environment.
2. It requires a large amount of data upfront for training.

# Online learning is preferred in circumstances such as

1. When the environment is dynamic and unpredictable, requiring real-time adaptation.
2. When the data is streaming and you can make decisions as the data arrives.
3. When the agent is capable of interacting with the environment safely while learning.
4. In interactive settings where the agent must react to user input.
5. When the policy needs to continuously improve and adapt to new situations.
6. When immediate adaptation to new data is required.


# Offline learning is preferred in circumstances such as:

1. When there is a large pre-existing dataset from which the agent can learn.
2. When learning in the actual environment is costly, dangerous, or unethical.
3. When the environment is static or changes very slowly or doesn't change at all.
4. In situations where online trial-and-error learning is not feasible or desirable.
5. When you need to reduce the variance of the learning process by using batch updates.
6. When a large amount of data is available upfront.
7. When there are computational or resource constraints.
8. 






# Applications of Online RL

1. High-frequency trading: Online RL can help make trading decisions in real-time based on the fluctuating market.
2. Adaptive control systems in robotics: Robots can use online RL to adapt to changing environments.
3. Personalized recommendations: Online RL can be used to adapt recommendations based on users' real-time behavior.

# Real-world applications of offline RL:

1. Customer behavior analysis: Offline RL can be used to analyze historical customer data to make future marketing strategies.
2. Healthcare: Offline RL can be used to analyze past patient data to make treatment recommendations.
3. Supply chain optimization: Using historical data, offline RL can optimize supply chain decisions.

# Advantages and Disadvantages of Training Surgical Robots Online

### Advantages:

1. Online learning could allow the robot to adapt to individual patient characteristics in real-time.
2. It could potentially lead to improved surgical outcomes by continuously improving performance.


### Disadvantages:

1. The risk of making errors that could potentially harm a patient is high.
2. It would be ethically and legally challenging to implement, as it could be considered experimentation on patients.
3. The high-stakes nature of surgery means that a high degree of certainty is required before actions are taken, which may not be possible with online learning.

# Reasons for using Offline RL for Surgical Robots

1. Safety: In a surgical setting, there is no room for error. Online learning, which adapts in real-time, can make mistakes that could be disastrous.
2. Ethics: It would be unethical to allow a surgical robot to learn and make mistakes on real patients.
3. Data availability: There are plenty of recorded surgeries and simulations that could be used for offline learning.

#### Exceptions: Instances where online RL might be preferred over offline RL for surgical robots

1. The robot needs to adapt to the unique physiology or conditions of each patient in real-time.
2. The surgical environment is highly dynamic or unpredictable and the robot needs to respond to these changes in real-time.

# RL in Self-Driving Cars

1. RL can help a self-driving car to learn optimal driving strategies from raw sensory input.
2. RL can also help the car adapt to changes in the environment, such as changing traffic conditions or new road layouts.
3. Companies like Waymo and Tesla use forms of RL to train their autonomous vehicles.

# Markov Property

1. refers to the memoryless property of a stochastic process - the future states depend only on the current state and not on the sequence of events that preceded it.
2. forms the basis for Markov Decision Processes (MDPs)
3. **Real-world examples generally do not strictly follow the Markov property. Most of the time, future states depend not only on the present state but also on past states. However, the Markov property is still used as a simplifying assumption to make problem-solving more tractable.**

# Assumptions of Markov Property

1. The future state is conditionally independent of the past given the present.
2. The transition probabilities (i.e., the probabilities of moving from one state to another) only depend on the current state and not the history of past states.

# Advantages of Markov Property

1. It simplifies the modeling process.
2. It reduces the computation required in the decision-making process.

# Disadvantages of Markov Property

1. It assumes the system is memoryless, which is not always true in real-world situations.
2. It might not be suitable for problems where the future state depends on the history of past states.

# Markov Decision Process

1. mathematical framework used for modeling decision making in situations where outcomes are partly random and partly under the control of a decision maker.
2. simplifies the modeling of the decision process, making it more computationally feasible to solve problems in RL.
3. **Real-world examples generally do not strictly follow either the Markov property or MDPs due to the complexity and randomness inherent in real-world situations. However, they are used as approximations to make problem-solving more tractable.**
4. **The environment is assumed to be fully observable in MDPs because it simplifies the problem. If the agent can fully observe the state of the environment, it can determine the optimal action to take. This makes the problem more tractable and enables the use of standard MDP algorithms.**
5. They are widely used in reinforcement learning to formally describe an environment for learning.
6. MDPs are used in various fields, including economics, game theory, control theory, operations research, and artificial intelligence.
7. They allow for the formal definition of policies and value functions in RL.

# Markov Property Vs MDP

1. Markov property is a characteristic of a stochastic process where the future states depend only on the current state and not on the sequence of events that preceded it.
2. An MDP is a model used for decision making that uses the Markov property. It includes not only the states and the transition probabilities between them but also the possible decisions (actions) and the rewards for each state-action pair.

# Advantages of MDP

1. They provide a formal mathematical framework for modeling decision-making in a variety of fields.
2. They simplify complex decision-making problems by using the Markov property.

# Disadvantages of MDPs:

1. They assume the Markov property, which isn't always valid in real-world situations.
2. They assume full observability of the environment, which is often not the case in reality.

# Can we Use MDPs in Partially Observable Environments?

1. j,

# POMDPS

1. POMDPs extend MDPs to handle partially observable environments.
2. POMDPs can model a wide range of real-world problems where the state of the environment isn't fully observable.
3. In POMDPs, the agent maintains a belief state, which is a probability distribution over the possible states of the environment, based on the history of observations, actions, and rewards.
4. Solving POMDPs is computationally challenging, so approximate methods are often used.
5. POMDPs can be applied in various areas such as robotics (where robots may have incomplete information about their environment), healthcare (where doctors may have incomplete information about a patient's health), and natural resource management (where managers may have incomplete information about the state of the environment).

# Reasons for having POMDPs when we have MDPs:

1. MDPs assume that the environment is fully observable, which is often not the case in real-world problems.
2. POMDPs extend MDPs to handle partially observable environments, making them more versatile for real-world problems.
3. POMDPs can handle uncertainty in both the state transitions and the observations, which is crucial in many situations.
