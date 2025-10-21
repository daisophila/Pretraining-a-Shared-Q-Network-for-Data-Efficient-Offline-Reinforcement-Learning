# Pretraining A Shared Q-Network for Data Efficient Offline Reinforcement Learning

With just a few modification, you can apply our method to all of offline RL algorithms. To show an example, we implemented it on TD3+BC. In the codes, we denoted what we modified.

### Environments
Our environment was set to python 3.9.12 pytorch 2.1.0+cu118.

### Usage
```
python main.py --pretrain True
```

If you want to reduce a dataset size, just add contraction_rate argument
### Pretraining and RL Training using 10% of Dataset
```
python main.py --pretrain True --contraction_rate 0.1
```
