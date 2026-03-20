---
layout: post
title: Defended my MS thesis. Title - "Towards safe and efficient offline reinforcement learning - learning safety constraints and expressive policies via generative modeling"
date: 2025-06-17 16:11:00-0400
inline: false
related_posts: false
---

Abstract:

---

Offline reinforcement learning (RL) presents a particularly challenging setting due to the lack of active environment interaction, making it critical to learn from static datasets in a way that both respects safety constraints and captures complex action distributions. This thesis investigates algorithmic advancements in offline reinforcement learning (RL) with a focus on (a) ensuring policy safety under uncertainty and (b) enhancing the expressiveness and efficiency of learned behaviors.

The first part of the thesis introduces a Latent Safety-Constrained Policy framework for safe offline RL. We address the inherent trade-off between safety enforcement and reward maximization by learning a latent representation of safety constraints using a Conditional Variational Autoencoder (CVAE). The learned latent space allows us to decouple safety modeling from reward learning. We then formulate a constrained reward-return maximization problem in this latent space, optimizing a policy via reward-weighted advantage regression that remains compliant with inferred safety boundaries. The proposed approach is grounded in theoretical analysis, including performance bounds and sample complexity estimates, and empirically validated on benchmark tasks, including high-risk autonomous driving scenarios. Results demonstrate significant improvements in both safety compliance and cumulative reward compared to existing baselines.

The second part of the thesis addresses the high inference cost and training instability of iterative generative policies, such as diffusion models, in offline RL. We propose the Single-Step Completion Policy (SSCP), a novel generative actor trained via an augmented flow-matching objective that directly predicts the action completion vector from intermediate flow states. SSCP eliminates the need for multistep sampling or long backpropagation chains, achieving one-shot action generation without sacrificing expressiveness. Integrated within an off-policy actor-critic framework, SSCP scales to both offline and offline-to-online RL settings. Further, this idea can be extended to goal-conditioned scenarios to exploit subgoal structures in long-horizon tasks without hierarchical decomposition. Experimental results across standard offline RL and behavior cloning benchmarks highlight SSCP’s strong performance, fast inference, and policy flexibility.

Collectively, these contributions offer scalable solutions to critical challenges in offline RL by enabling safe, efficient, and expressive policy learning. The methods developed in this thesis lay the foundations for the deployment of RL agents in real-world applications with resources and safety constraints.

---
