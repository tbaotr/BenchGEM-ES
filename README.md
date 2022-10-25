# Benchmarking Gradient Estimation Mechanisms in Evolution Strategies for Solving Black-Box Optimization Functions and Reinforcement Learning Problems
[![MIT licensed](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE.md)

Thai Bao Tran, Ngoc Hoang Luong

## Setup
- Clone this repo:
```
$ git clone ...
$ cd BenchGEM-ES
```

- Install dependencies:
```
$ pip install -r requirements.txt
```
To perform experiments on RL, we install MuJoCo from [here](https://github.com/openai/mujoco-py)

## Usage

### Run

- For BBOB:
  - Move all files from outside to /scripts/bbob/
  - Run bash files with our settings

```
bash run_es.sh
bash run_ges.sh
bash run_sges,sh
```
- For RL:
  - Move all files from outside to /scripts/rl/vi/ (i is the version needed to perform)
  - Run bash files with our settings
```
bash run_es.sh
bash run_ges.sh
bash run_sges,sh
```

### Evaluate & Visualize

- With folder *log* including files containing history of optimization process, run this command to get the synthetic files:

```
python aggregate.py
```

- To visualize the synthetic files:

```
python plot.py
```


## Acknowledgement
Our source code is inspired by:
- [Guided Evolutionary Strategy](https://github.com/brain-research/guided-evolutionary-strategies)
- [Self-Guided Evolutionary Strategy](https://github.com/IJCAI2020-SGES/SGES)
- [pycma: CMA-ES in Python](https://github.com/CMA-ES/pycma)
- [Evolution Strategies as a Scalable Alternative to Reinforcement Learning](https://github.com/openai/evolution-strategies-starter)
