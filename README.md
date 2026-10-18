# Reinforcement Learning Notebooks

Jupyter notebooks implementing classic tabular reinforcement learning algorithms.

## Notebooks

| Notebook | Topic | Setting |
|----------|--------|---------|
| [`MAB.ipynb`](MAB.ipynb) | Multi-armed bandits | Exploration–exploitation ($k$-armed bandit, stationary / non-stationary) |
| [`MDP.ipynb`](MDP.ipynb) | MDPs & dynamic programming | Value iteration and policy iteration on a GridWorld (known model) |
| [`Monte_Carlo.ipynb`](Monte_Carlo.ipynb) | Monte Carlo methods | Policy evaluation and control on Blackjack (no model, full episodes) |
| [`Temporal-difference.ipynb`](Temporal-difference.ipynb) | Temporal-difference control | SARSA and Q-learning on FrozenLake (no model, online bootstrapping) |

Suggested order: **MAB → MDP → Monte Carlo → Temporal-difference**.

## Requirements

- Python 3.10+
- [Jupyter](https://jupyter.org/) / VS Code / Cursor notebook support

```bash
pip install numpy matplotlib gymnasium
```

Optional (for interactive displays in the TD notebook):

```bash
pip install ipython
```

## How to run

```bash
jupyter notebook
# or
jupyter lab
```

Then open any `.ipynb` file and run the cells top to bottom.

## What each notebook covers

- **MAB** — $\varepsilon$-greedy, UCB, gradient bandit; regret and average reward curves
- **MDP** — Bellman backups, value / policy iteration, policy extraction, GridWorld visualization
- **Monte Carlo** — first-visit / every-visit evaluation, exploring starts, on-policy and off-policy control
- **Temporal-difference** — $\varepsilon$-greedy behavior, SARSA (on-policy), Q-learning (off-policy)

## References

1. S. Airiau. *Apprentissage par renforcement*. M2 IASD, Université Paris Dauphine.  
   [https://www.lamsade.dauphine.fr/~airiau/Teaching/M2-IASDapp-RL/](https://www.lamsade.dauphine.fr/~airiau/Teaching/M2-IASDapp-RL/)
2. R. S. Sutton and A. G. Barto. *Reinforcement Learning: An Introduction*, 2nd ed. MIT Press, 2018.
