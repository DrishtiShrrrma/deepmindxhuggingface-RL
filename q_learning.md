
# Policy

1. Agent's brain - defines agent's behaviour
2. a policy outputs an action or a probability distribution over actions that an agent should take in a given state
3. goal: to find an optimal policy that leads to high cumulative reward

# Methods to Find Optimal Policy

1. Policy-based methods: policy is trained directly to learn which action to take given a state    (state --> action)
2. Value-based methods: a value func is trained to learn which state is more valuable and then value function is used to take the action that leads to it. (state ---> value)
