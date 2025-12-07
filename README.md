# **Jackpot: Optimal Budgeted Rejection Sampling for Extreme Actor–Policy Mismatch RL**

**Official repository for _Jackpot_.**

**Authors:**  
**Zhuoming Chen\***, **Hongyi Liu\***, **Yang Zhou\***, Haizhong Zheng, Beidi Chen  
*Carnegie Mellon University*  
(\* = Equal Contributions, alphabetically ordering based on lastnames) 

[📄 **Download Paper (PDF)**](https://github.com/Infini-AI-Lab/jackpot/blob/main/jpt.pdf) 

---

## **Abstract**

Reinforcement learning (RL) for large language models (LLMs) remains expensive, particularly because
the rollout is expensive. Decoupling rollout generation from policy optimization (e.g., leveraging a
more efficient model to rollout) could enable substantial efficiency gains, yet doing so introduces severe
distribution mismatch that destabilizes learning. We propose Jackpot, a framework that leverages
Optimal Budget Rejection Sampling (OBRS) to directly reduce the discrepancy between the rollout
model and the evolving policy. Jackpot integrates a principled OBRS procedure, a unified training
objective that jointly updates the policy and rollout models, and an efficient system implementation
enabled by top-k probability estimation and batch-level bias correction. Our theoretical analysis
shows that OBRS consistently moves the rollout distribution closer to the target distribution under
a controllable acceptance budget. Empirically, Jackpot substantially improves training stability
compared to importance-sampling baselines, achieving performance comparable to on-policy RL when
training Qwen3-8B-Base for up to 300 update steps. Taken together, our results show that OBRS-based
alignment brings us a step closer to practical and effective decoupling of rollout generation from policy
optimization for RL for LLMs.

## **Bibliography** 

If you think our work is helpful, please consider citing us using the following BibTeX. 

```bibtex
@misc{jackpot2025github,
  title        = {Jackpot: Optimal Budgeted Rejection Sampling for Extreme Actor-Policy Mismatch RL},
  author       = {Liu, Hongyi and Chen, Zhuoming and Zhou, Yang and Zheng, Haizhong and Chen, Beidi},
  howpublished = {\url{https://github.com/Infini-AI-Lab/jackpot.git}},
  note         = {Official GitHub repository},
  year         = {2025}
}
