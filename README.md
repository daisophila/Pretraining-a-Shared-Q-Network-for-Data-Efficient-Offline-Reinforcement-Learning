# Pretraining A Shared Q-Network for Data Efficient Offline Reinforcement Learning

With just a few modification, you can apply our method to all of offline RL algorithms. To show an example, we implemented it on TD3+BC. In the codes, we denoted what we modified.

### Environments
Our environment was set to python 3.9.12 pytorch 2.1.0+cu118.

### Usage
```
python main.py --pretrain True --pretrain_rate 0.1
```

If you want to reduce a dataset size, just add contraction_rate argument
```
python main.py --pretrain True --pretrain_rate 0.1 --contraction_rate 1.0
```
