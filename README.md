# Deep Reinforcement Learning–Based Routing Optimization

This project implements a **Deep Reinforcement Learning (DRL)** approach for intelligent network routing. It combines a traditional cost-based routing baseline with a **Deep Q-Network (DQN)** model and an interactive frontend to analyze, compare, and visualize routing behavior under multiple network constraints.

---

## Dataset

The project uses a **Multi-Criteria Network Routing Dataset** designed for research on secure, reliable, and efficient data transmission in distributed networks. The dataset supports the development and evaluation of routing optimization algorithms by incorporating both performance and security-related factors.

The dataset contains **500 simulated routing records**, where each route is evaluated using metrics such as latency, bandwidth, security risk, trust score, packet delivery ratio, end-to-end delay, and energy consumption. A target column, **Optimal_Route**, labels each route as **Optimal (1)** or **Non-Optimal (0)** based on predefined multi-criteria conditions.

**Key dataset features:**
- Route characteristics: source node, destination node, latency, bandwidth  
- Security metrics: security risk score, trust score  
- Performance indicators: packet delivery ratio, end-to-end delay, energy consumption  
- Target label: Optimal vs Non-Optimal routing decision  

**Dataset usage:**  
Download the dataset from the provided link, upload it to a **Google Colab notebook**, and execute the code cells sequentially to reproduce the experiments.

---

## Coding Implementation

The coding component implements a complete **DRL-based routing pipeline** using Python. The workflow begins with dataset loading, cleaning, and normalization to ensure numerical stability during learning.

A traditional **cost-based routing baseline** is implemented using weighted routing metrics to serve as a reference model. The routing problem is then formulated as a reinforcement learning task by defining the state space, action space, and a multi-objective reward function that balances latency, reliability, energy efficiency, and trust.

A **Deep Q-Network (DQN)** is used to approximate the action-value function. The model is trained using an epsilon-greedy exploration strategy and gradient-based optimization. Learning behavior is analyzed using reward convergence plots, and a fair comparison is performed between traditional routing and DRL-based routing. The trained model is finally used to select the optimal routing path based on learned experience.

---

## Frontend Implementation

The frontend provides an interactive visualization of the DRL-based routing system. It visually represents network topology, routing paths, congestion levels, and packet flow in real time. The frontend also displays learning metrics such as reward progression and enables comparison between traditional routing and DRL-based routing behavior.

This component serves as a visual and analytical tool to understand how the DRL agent learns, adapts to changing network conditions, and improves routing decisions over time. The frontend complements the core algorithmic implementation by making the learning process and routing outcomes intuitive and easy to analyze.

---

## Academic Context

This project was developed as part of a **B.Tech Artificial Intelligence and Data Science academic project**, focusing on:
- Intelligent routing algorithms  
- Reinforcement Learning and Deep Reinforcement Learning  
- Multi-objective optimization  
- Visualization of learning-based systems  

---

## Notes

- The repository contains the **core experimental and algorithmic code**.
- The frontend is included or referenced separately as part of the project demonstration.
- The project is intended for **educational and research purposes**.
