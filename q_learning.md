
# Policy

1. Agent's brain - defines agent's behaviour
2. a policy outputs an action or a probability distribution over actions that an agent should take in a given state
3. goal: to find an optimal policy that leads to high cumulative reward

# Methods to Find Optimal Policy

1. Policy-based methods: policy is trained directly to learn which action to take given a state    (state --> action)
- policy = NN
- no value func
- state (input) ---> action (output)

![image](https://github.com/DrishtiShrrrma/deepmindxhuggingface-RL/assets/129742046/c93991a8-d901-4d58-8bbb-261c1f965066)


2. Value-based methods: a value func (NN) is trained to learn which state is more valuable and then value function is used to take the action that leads to it. (state ---> value)
- The value of a state is the expected discounted return the agent can get if it starts at that state and then acts according to a policy.


![image](https://github.com/DrishtiShrrrma/deepmindxhuggingface-RL/assets/129742046/ba662aa0-43e2-488e-8aac-c35152b69366)

### Crux

1. In policy-based training, the optimal policy (π*) is found by training the policy directly.
2. In value-based training, finding an optimal value function (Q* or V*) leads to having an optimal policy.

# Stochastic Vs Deterministic Policy


# Bellman Equation

1. by Richard Bellman
2. it defines the value function of a policy as the sum of expected immediate rewards plus the expected values of the subsequent states.
3. instead of calculating each value as the sum of the expected return, which is a long process, we calculate the value as the sum of immediate reward + the discounted value of the state that follows.
4. Can represent both deterministic and stochastic environments.
5. can be applied to both continuous and discrete action spaces. In continuous action spaces, additional methods like function approximation may be needed.
6. offers a recursive way to calculate the value of a state. Instead of calculating the expected return for each state from scratch, it considers the immediate reward plus the discounted value of the following state. 
7. Basis for algorithms in planning and decision-making tasks.

![image](https://github.com/DrishtiShrrrma/deepmindxhuggingface-RL/assets/129742046/1a1b759f-0fa0-4a46-ae7b-1cdbe17c5ccb)

# Assumptions of Bellman Equation

1. Markov Property: Future states depend only on the current state and action.
2. Stationarity: Transition probabilities and rewards remain the same over time.
3. Fully Observable State: All relevant information is captured in the state.

# Limitations of Bellman Equation

1. Can be computationally expensive for large state spaces.
2. Requires the system to have the Markov property, which might not hold in some real-world scenarios.

# Determinisitic Vs Stochastic Envio

1. Deterministic Environment: Chess - outcome of an action is entirely predictable.
2. Stochastic Environment: Stock market trading -  outcome of buying or selling is not entirely predictable.

# Monte Carlo Approach

1. estimates value functions by averaging over many sample returns, based on actual experiences.
2. value of states or state-action pairs without assuming complete knowledge of the environment.
3. Powerful in model-free environments and can provide unbiased estimates.
4. Doesn't require a model of the environment.
5. Has high variance but unbiased estimates.
6. simplicity in implementation

# Disadvantages of Monte Carlo Approach

1. High Variance
2. Requires the completion of an episode to update values.

# Temporal Difference Learning

1. combination of Monte Carlo and Dynamic Programming methods. It updates value estimates based on the difference between consecutive estimates.
2. Efficiently leverages partial information and is more computationally efficient than Monte Carlo.

# Advantages of Temporal Difference Learning

1. Lower variance.
2. Can learn from incomplete sequences (online learning).
3. Typically more computationally efficient.

# Disadvantages of TD Learning

1. Introduces bias into estimates.
2. More complex in formulation compared to Monte Carlo.

# Monte Carlo Vs Temporal Difference Learning:

1. Monte Carlo: Waits until the end of an episode to update value estimates (val func) - so the actual accurate discounted return of this episode is used - has high variance.
2. Temporal Difference Learning: Updates value estimates at each time step - we replace Gt with TD target (estimated return) - reduces variance but introduces bias.


![image](https://github.com/DrishtiShrrrma/deepmindxhuggingface-RL/assets/129742046/4f0ec64d-fb31-4ec4-b67a-216ddc3a1399)



# Bias Vs Variance

1. Aj
2. Analogy: In a college class, bias is like a professor who always grades a bit too harshly. Variance is like a professor who sometimes grades too easy and sometimes too hard. Need: a balance where the grades are fair (low bias) and consistent (low variance).

# Q-learning

1. a model-free reinforcement learning algorithm used to find the optimal action-selection policy for a given finite MDP by learning a value function.
2. doesn't require a model of the environment.
3. Q in Q-learning stands for "Quality." It represents the quality of a particular action in a given state.
4. Q-table is a lookup table where the Q-values are stored for each state-action pair.
5.  one of the first successful algorithms to learn directly from high-dimensional sensory inputs.

# Assumptions related to Q-learning

1. The environment must be a finite Markov decision process.
2. A finite set of states and actions.
3. Rewards are assumed to have bounded values - helps in maintaining numerical stability, avoiding extremely large Q-values that may lead to divergence.
4. 

# Advantages of Q-Learning:

1. It is model-free.
2. It can handle problems with stochastic transitions and rewards.
3. It converges to the optimal policy given enough exploration.

# Disadvantages of Q-Learning:

1. It can be slow to converge in large state spaces.
2. Can suffer from the "curse of dimensionality."
3. It requires careful tuning of hyperparameters.

# Limitations of Q-Learning:

1. Requires discretization in continuous state/action spaces.
2. Exploration vs exploitation must be balanced.
3. Sensitive to initial parameter settings.
4. 

# Applications of Q-learning

1. Controlling a self-driving car.
2. Managing investment portfolios.
3. Teaching a computer agent to play games like Pac-Man or Tic-Tac-Toe.
