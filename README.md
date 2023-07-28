# Reinforcement Learning

1. type of machine learning where an agent learns to make decisions by taking actions in an environment. The agent is rewarded or penalized (gets positive or negative reinforcement), based on the results of its actions. The aim is to maximize the cumulative reward over time.
2. RL is about sequential decision making, aiming to choose a series of actions that maximizes some reward
3. 

![image](https://github.com/DrishtiShrrrma/coherexhuggingface-RL/assets/129742046/b401dddb-605d-46b0-9fce-a503d5f95f58)


# Reinforcement Learning Vs Supervised Learning

1. In supervised learning, the output corresponding to each input during training while in reinforcement learning, no such output is provided.
2. RL is about sequential decision making, aiming to choose a series of actions that maximizes some reward, while supervised learning is about mapping inputs to outputs.
3. RL involves an environment, states, actions, and rewards, while supervised learning involves input data and corresponding labels.

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

1. When the environment is dynamic and changes over time.
2. When new data is constantly becoming available.
3. When immediate adaptation to new data is required.

# Offline learning is preferred in circumstances such as:

1. When the environment is static or changes very slowly.
2. When a large amount of data is available upfront.
3. When there are computational or resource constraints.


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

# Surgical Robots 
4. 
