# cs370-portfolio
# CS-370: Reinforcement Learning – Treasure Hunt Pirate Agent  
**Author:** Shah Ali Omor  
**Project:** Deep Q-Learning Intelligent Pirate Agent  

---

## Project Overview
In this project, I developed an intelligent pirate agent that learns to locate treasure in a maze before the human player. The objective was to apply reinforcement learning and neural-network principles to create a non-player character (NPC) that improves its decision-making through repeated experience.

The environment represents a maze with pathways and obstacles. The pirate receives rewards for moving closer to the treasure and penalties for hitting walls or wasting moves. Through a Deep Q-Learning (DQN) neural network built with Keras and TensorFlow, the agent gradually learned to navigate toward the optimal strategy by trial and error.

---

## Code Summary
I was provided with a working framework to guide the structure of my implementation:
- **Given files:**  
  - `TreasureHuntGame.ipynb` – contained the project’s initial notebook setup and basic cell structure for loading, training, and testing the agent.  
  - `TreasureMaze.py` – defined the maze environment, including rules, rewards, and penalties.  
  - `GameExperience.py` – implemented the replay-memory buffer that stored past experiences for training.  

I created and customized the core parts of the project:
- **My contributions:**  
  - Designed and tuned the **`qtrain()`** function that managed the full training process for the DQN agent.  
  - Adjusted **hyperparameters** such as learning rate, discount factor, exploration decay, and batch size for performance stability.  
  - Modified sections of the notebook to **suppress verbose outputs**, log results after each epoch, and ensure smooth execution in Jupyter without kernel crashes.  
  - Executed full training over **999 epochs (~12.5 hours)**, achieving a **final loss ≈ 0.0206** and **win rate ≈ 0.094 (73 wins / 1000 episodes)**.  

These steps demonstrated the effectiveness of reinforcement learning through self-improvement without explicit external direction.

---

## Connecting Learning to the Field of Computer Science

### What do computer scientists do, and why does it matter?
Computer scientists design intelligent, data-driven systems that solve complex real-world problems. By building this project, I saw how reinforcement learning mirrors human trial-and-error reasoning, enabling technology to adapt autonomously. This skill is vital for areas like robotics, self-driving vehicles, and game AI—fields where independent learning and optimization make a major impact.

### How do I approach a problem as a computer scientist?
I approach problems analytically and iteratively. I start by understanding requirements, then build solutions in modular steps, test thoroughly, and refine based on data. In this project, that meant debugging environment code, adjusting DQN parameters, and re-running training sessions until the model behaved as expected. This cycle of hypothesis, testing, and refinement defines how I approach all computational challenges.

### What are my ethical responsibilities to the end user and the organization?
As a computer scientist, I must ensure that intelligent systems behave safely, fairly, and transparently. AI solutions should respect privacy, avoid biased decision-making, and serve both the user and organizational integrity. Reinforcement learning models—like the pirate agent—should be designed with predictable boundaries so they act ethically within defined rules.

---

## Reflection
Completing this Deep Q-Learning project gave me a deeper appreciation for how AI can learn autonomously through experience. I learned to handle performance bottlenecks, interpret neural feedback, and manage large-scale training tasks efficiently. Beyond the technical lessons, it strengthened my understanding of responsible innovation—building systems that not only perform well but also align with ethical and human-centered computing values.
