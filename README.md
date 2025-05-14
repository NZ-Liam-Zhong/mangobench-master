<div id="user-content-toc">
  <ul align="center" style="list-style: none;">
    <summary>
      <h1>MangoBench: Benchmarking Multi-Agent Goal-Conditioned Offline Reinforcement Learning</h1>
    </summary>
  </ul>
</div>

<div align="center">
<img src="assets/mangobench.png" width="900px"/>



</div>

# Overview
Goal-conditioned offline reinforcement learning is an important field in modern reinforcement learning for its simplicity and universality.It is especially essential in multi-agent settings, where manually designing or shaping rewards is notoriously difficult, and iteratively collecting experience through environmental interaction is both costly and risky. Despite its importance in multi-agent settings, there is currently a lack of algorithms. Therefore, we propose MangoBench, the first multi-agent goal-conditioned offline reinforcement learning benchmark. MangoBench consists of $3$ environments, $4$ types of agents, $51$ tasks with different levels of challenges and $3$ baseline algorithms designed by ourselves, including goal-conditioned multi-agent behavior cloning, independent contrastive reinforcement learning, and independent hierarchical implicit Q-learning. Experiments demonstrate that independent hierarchical implicit Q-learning emerges as the state-of-the-art algorithm for multi-agent offline goal-conditioned tasks among the three baseline algorithms. We hope that this benchmark can contribute to the multi-agent learning academic field.

MangoBench is a multi-agent goal-conditional offline RL benchmark. Our benchamrk is based on [MUJOCO](https://github.com/google-deepmind/mujoco),[MaMujoco](https://robotics.farama.org/envs/MaMuJoCo/index.html),[OGBench](https://seohong.me/projects/ogbench/).

# Comparison with other Multi-agent Benchmark
<div align="center">
<img src="assets/comparison_benchmark.png" width="900px"/>
</div>

# How to use the MANGOBench environments

### Installation

MangoBench follow the environment and datasets of [OGBench](https://seohong.me/projects/ogbench/).



### Algorithms
We offer three algorithms for baselines.

1. ICRL (Independent Contrastive Reinforcement Learning): Located in ```impls/agents/crl.py```
2. MAGCBC (Multi-agent Goal-Conditional Behaviour Cloning): Located in ```impls/agents/gcbc.py```
3. IHIQL (Independent Hierarchical Implicit Q-Learning): Located in ```impls/agents/hiql.py```

### How to run the code
We can run the code by running the bash file: ```bash impls/hyperparameters_multi.sh```

# WandB Evaluation
<div align="center">
<img src="assets/wandb.png" width="500px"/>
</div>

# Results
<div align="center">
<img src="assets/results.png" />
</div>