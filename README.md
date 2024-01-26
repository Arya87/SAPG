# Self-Adaptive Policy Guiding (SAPG): Enhancing Model-based Reinforcement Learning with Expert Demonstrations for sparse-rewarded Tasks

Original PyTorch implementation of Self-Adaptive Policy Guiding (SAPG): Enhancing Model-based Reinforcement Learning with Expert Demonstrations for sparse-rewarded Tasks.




## Instructions

We assume that your machine has a CUDA-enabled GPU, a local copy of MuJoCo 2.1.x installed (required for the Adroit/Meta-World domains), and at least 80GB of memory. Then, create a conda environment with `conda env create -f environment.yml`, and add `/<path>/<to>/<your>/modem/tasks/mj_envs` to your `PYTHONPATH` (required for the Adroit domain). You will also need to configure `wandb` and your demonstration/logging directories in `cfgs/config.yaml`. Demonstrations are made available [here](https://github.com/facebookresearch/modem/releases/tag/v.0.1.0). Once setup is complete, you should be able to run the following commands.

To train SAPG on a task from **Adroit**:

```
python train.py suite=adroit task=adroit-door
```

To train SAPG on a task from **Meta-World**:

```
python train.py suite=mw task=mw-assembly
```


## Acknowledgements

Our code is based on [MoDem](https://nicklashansen.github.io/modemrl) .
