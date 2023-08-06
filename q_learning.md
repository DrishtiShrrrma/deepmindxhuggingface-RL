
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
6. Basis for algorithms in planning and decision-making tasks.

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

