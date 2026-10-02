# 🎰 Reinforcement Learning

Solve the **multi-armed bandit** problem: learn which option is best while you are still collecting data.

| Notebook | Algorithm | Key idea |
|----------|-----------|----------|
| [upper_confidence_bound.ipynb](upper_confidence_bound.ipynb) | Upper Confidence Bound (UCB) | Deterministic: picks the ad with the highest optimistic estimate |
| [thompson_sampling.ipynb](thompson_sampling.ipynb) | Thompson Sampling | Probabilistic: samples from a Beta distribution for each ad |

## 📊 Dataset: `Ads_CTR_Optimisation.csv`

A simulation of **10 ad versions** shown to **10,000 users**. Each cell is `1` if the user would click that ad, `0` otherwise.

**Goal:** find the ad with the highest click-through rate (CTR) while maximising total clicks along the way.

## 🎯 Result

Both algorithms converge on the same best ad. **Thompson Sampling** usually finds it with fewer rounds than UCB.
