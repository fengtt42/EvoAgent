# EvoAgent: Agent Autonomous Evolution with Continual World Model for Long-Horizon Tasks


The reimplementation of [EvoAgent](https://arxiv.org/pdf/2502.05907), an autonomous-evolving agent with a continual World Model (WM), which can autonomously complete various LH tasks across environments through self-planning, self-control, and self-reflection, without human intervention. 


![2.png](Pics%2F2.png)
>EvoAgent, the first autonomous-evolving agent with a continual World Model (WM). Take Minecraft as an example. 
>Left: Various Long-Horizon (LH) tasks across environments. 
>Middle: EvoAgent includes a memory-driven planner, a WM-guided action controller, and an experience-inspired reflector. EvoAgent can autonomously complete various LH tasks across environments by selfplanning, self-control, and self-reflection, without human intervention. 
>Right: We build a continual WM for EvoAgent. Through closed-loop dynamics, EvoAgent can continuously update the multimodal experience pool and world knowledge.

##  📚 Embodied AI Paper Lists

Completing Long-Horizon (LH) tasks in open-ended worlds is an important yet difficult problem for embodied agents.


> Existing approaches suffer from two key challenges: 
> 
(1) they heavily rely on experiences obtained from human-created data or curricula, lacking the ability to continuously update multimodal experiences

(2) they may encounter catastrophic forgetting issues when faced with new tasks, lacking the ability to continuously update world knowledge. 

To solve these challenges, this paper presents _EvoAgent_, an autonomous-evolving agent with a continual World Model (WM), which can autonomously complete various LH tasks across environments through self-planning, self-control, and self-reflection, without human intervention. 

Our proposed EvoAgent contains three modules, i.e., i) the memory-driven planner which uses an LLM along with the WM and interaction memory, to convert LH tasks into executable sub-tasks; ii) the WM-guided action controller which leverages WM to generate low-level actions and incorporates a self-verification mechanism to update multimodal experiences; iii) the experience-inspired reflector which implements a two-stage curriculum learning algorithm to select experiences for task-adaptive WM updates. 

Moreover, we develop a continual World Model for EvoAgent, which can continuously update the multimodal experience pool and world knowledge through closed-loop dynamics. 

We conducted extensive experiments on Minecraft, compared with existing methods, EvoAgent can achieve an average success rate improvement of 105% and reduce ineffective actions by more than 6x.

The list is designed to help you build a solid worldview of the field, guiding you from foundational concepts to advanced topics, and from broad perspectives to specific technical challenges. <font color=yellow>Please read in order.</font>



##  🗺️ World Model Paper Lists

The world model architectures of autonomous embodied agents include RSSM, JEPA, Transformer, Diffusion, and Hierarchical.

##  🚀 Long-Horizon Task Paper Lists


##  🎯 Reference

```bibtex
@article{feng2025evoagent,
  title={EvoAgent: Agent Autonomous Evolution with Continual World Model for Long-Horizon Tasks},
  author={Tongtong Feng and Xin Wang and Zekai Zhou and Ren Wang and Yuwei Zhan and Guangyao Li and Qing Li and Wenwu Zhu},
  journal={arXiv preprint arXiv:2502.05907},
  year={2025}
}
```


## Other Related Repos
[Awesome-World-Model](https://github.com/LMD0311/Awesome-World-Model),
[Awesome-World-Models-for-AD ](https://github.com/zhanghm1995/awesome-world-models-for-AD?tab=readme-ov-file#Table-of-Content),
[World models paper list from Shanghai AI lab](https://github.com/OpenDriveLab/End-to-end-Autonomous-Driving/blob/main/papers.md#world-model--model-based-rl),
[Awesome-Papers-World-Models-Autonomous-Driving](https://github.com/chaytonmin/Awesome-Papers-World-Models-Autonomous-Driving).
    
