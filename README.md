# EvoAgent: Agent Autonomous Evolution with Continual World Model for Long-Horizon Tasks


The reimplementation of [EvoAgent](https://arxiv.org/pdf/2502.05907), an autonomous-evolving agent with a continual World Model (WM), which can autonomously complete various LH tasks across environments through self-planning, self-control, and self-reflection, without human intervention. 

<div align=center>
    <img src="./Pics/1.png" width = 100% height = 100% />
</div>

>EvoAgent, the first autonomous-evolving agent with a continual World Model (WM). Take Minecraft as an example. 
>Left: Various Long-Horizon (LH) tasks across environments. 
>Middle: EvoAgent includes a memory-driven planner, a WM-guided action controller, and an experience-inspired reflector. EvoAgent can autonomously complete various LH tasks across environments by self-planning, self-control, and self-reflection, without human intervention. 
>Right: We build a continual WM for EvoAgent. Through closed-loop dynamics, EvoAgent can continuously update the multimodal experience pool and world knowledge.

#  🚀 Model Struction
EvoAgent contains three modules, i.e., i) the memory-driven planner which uses an LLM along with the WM and interaction memory, to convert LH tasks into executable sub-tasks; ii) the WM-guided action controller which leverages WM to generate low-level actions and incorporates a self-verification mechanism to update multimodal experiences; iii) the experience-inspired reflector which implements a two-stage curriculum learning algorithm to select experiences for task-adaptive WM updates.

<div align=center>
    <img src="./Pics/2.png" width = 50% height = 50% />
</div>

EvoAgent develops a continual World Model for EvoAgent, which can continuously update the multimodal experience pool and world knowledge through closed-loop dynamics. 

<div align=center>
    <img src="./Pics/4.png" width = 100% height = 100% />
</div>

EvoAgent conducted extensive experiments on Minecraft, compared with existing methods, EvoAgent can achieve an average success rate improvement of 105% and reduce ineffective actions by more than 6x.

<div align=center>
    <img src="./Pics/5.png" width = 100% height = 100% />
</div>


#  🗺️ Instructions

The code has been tested on Linux and requires Python 3.11+. This codebase is based on [dreamerv3](https://github.com/danijar/dreamerv3?tab=readme-ov-file).

###  Docker
You can either use the provided *Dockerfile* that contains instructions or follow the manual instructions below.

###  Manual
Training script:
```html
python EvoAgent/main.py \
  --logdir ~/logdir/{timestamp} \
  --configs Minecraft \
  --run.train_ratio 64
```

##  🎯 Reference
If you find this code useful, please reference in your paper:

```bibtex
@article{feng2025evoagent,
  title={EvoAgent: Agent Autonomous Evolution with Continual World Model for Long-Horizon Tasks},
  author={Tongtong Feng and Xin Wang and Zekai Zhou and Ren Wang and Yuwei Zhan and Guangyao Li and Qing Li and Wenwu Zhu},
  journal={arXiv preprint arXiv:2502.05907},
  year={2025}
}
```


## Other Related Repos
[dreamerv3](https://github.com/danijar/dreamerv3?tab=readme-ov-file),
[Awesome-Autonomous-Embodied-AI-from-Scratch](https://github.com/fengtt42/Awesome-Autonomous-Embodied-AI-from-Scratch),
[Awesome-World-Model](https://github.com/LMD0311/Awesome-World-Model)
