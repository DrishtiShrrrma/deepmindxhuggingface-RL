
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


# Stochastic Vs Deterministic Policy

