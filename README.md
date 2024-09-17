# 🚗 **Simulated Autonomous Driving AI using Reinforcement Learning** 💡

This repository contains a study and implementation of an AI-driven autonomous car in a simulated environment using **Reinforcement Learning**, specifically the **Q-Learning** algorithm. The project aims to demonstrate how an AI agent learns to make optimal driving decisions—such as lane selection, speed control, and obstacle avoidance—in a dynamic and ever-changing environment.

---

## 📋 **Key Features of the Study**

- **Agent-Based Learning**: The AI acts as an autonomous car that learns from its environment (simulated road with traffic obstacles).
- **Reinforcement Learning**: Utilizes Q-Learning to adapt the AI's behavior to maximize rewards and minimize penalties over time.
- **Dynamic Decision Making**: AI learns to choose actions like accelerating, decelerating, and lane-changing based on its state and received rewards.
- **Continuous Improvement**: Through trial and error, the AI continually improves its driving strategy to avoid collisions and reach its destination efficiently.

---

## 🎯 **Purpose**

To explore and understand the principles of **Reinforcement Learning** in autonomous driving applications and provide an educational example for those interested in AI, Machine Learning, and game simulation.

---

## 🧩 **How AI Learns in the Simulated Driving System**

The AI in this simulated driving system uses **Reinforcement Learning**, a technique in Machine Learning that allows AI to learn the best way to operate in a constantly changing environment. This learning process involves giving rewards or penalties to encourage the AI to adjust its behavior based on different situations it encounters.

### **Fundamental Principles of Reinforcement Learning:**

- **Agent**: The AI acts as the agent responsible for driving the car.
- **Environment**: The simulated road, with its various obstacles and conditions (such as Bot Cars), represents the environment the AI must navigate.
- **Actions**: The decisions made by the AI, such as choosing a lane, accelerating or decelerating, and changing lanes to avoid obstacles.
- **State**: The information the AI receives from the environment, including its position on the road, the distance to the car ahead, its current speed, and collision status.
- **Reward**: The score or reward the AI receives for safe driving and reaching the goal, or the penalties incurred when it crashes or goes off the road.

### **Algorithm Used for AI Learning**

The AI uses **Q-Learning**, a fundamental algorithm in Reinforcement Learning that aims to find the best policy for each state to maximize the total reward over the long term.

---

## 🔍 **How Q-Learning Works**

1. **Q-Table**:  
   A table used to store the expected reward values for each state-action pair. This table is gradually filled and updated during the learning process.

2. **Action Selection**:  
   The AI chooses an action in each state based on the values stored in the Q-Table. It may select the action with the highest expected reward (exploitation) or explore a new action to find a potentially better choice (exploration).

3. **Updating the Q-Table**:  
   Every time the AI takes an action and receives a reward or penalty, the values in the Q-Table are updated according to the formula:

   \[
   Q(s, a) \leftarrow Q(s, a) + \alpha [r + \gamma \max Q(s', a') - Q(s, a)]
   \]

   - \( s \): Current state  
   - \( a \): Action chosen  
   - \( r \): Reward received from taking the action  
   - \( s' \): New state after taking the action  
   - \( \alpha \): Learning rate  
   - \( \gamma \): Discount factor  

4. **Continuous Learning**:  
   The AI continuously learns by experimenting in the simulated environment, trying to improve its actions to maximize rewards and minimize penalties.

---

## 🧠 **How AI Learns in This Example**

In the simulated system, the AI learns through a process of repetition and testing:

- **Exploration and Experimentation**: The AI starts by randomly selecting different actions, such as accelerating, decelerating, changing lanes, or staying in its current lane, without initially knowing which choice is the best.
- **Receiving Rewards and Penalties**: As the AI drives in the simulated environment, it receives rewards for safe driving and reaching the goal (e.g., increasing the distance it must travel). It also receives penalties for crashing or going off the road.
- **Updating the Q-Table**: Whenever a crash occurs or the AI reaches its goal, the Q-Table is updated. This helps the AI learn what actions to take in various situations to maximize future rewards.
- **Long-Term Learning**: As the AI gains more experience, it can make better decisions, such as knowing when to change lanes or accelerate to reduce the risk of collision and reach its goal safely and quickly.

---

## 📊 **Example of AI Decision-Making**

- **Long Distance to Travel**: The AI may choose to stay in its current lane and maintain a speed close to the required average.
- **Obstacle Detection**: If the AI detects a Bot Car approaching, it might decide to change lanes to avoid a collision.
- **Near the Goal**: The AI may choose to speed up to reach the goal as quickly as possible.

---

## 🏁 **Conclusion**

The AI in this simulated driving system uses **Reinforcement Learning** with the **Q-Learning** algorithm to improve its driving decisions. It learns through trial and error, accumulating experience, and updating the best actions based on the situations encountered in the virtual environment. Over time, the AI can adapt and improve its driving skills, reducing the chance of collisions and increasing the likelihood of reaching the goal quickly and safely.

---

## 🛠️ **Keywords**

`Autonomous Driving`, `AI`, `Reinforcement Learning`, `Q-Learning`, `Simulation`, `Python`, `Pygame`

## 📜 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📚 **Resources and Further Reading**

- [Reinforcement Learning: An Introduction](https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf)
- [Q-Learning Algorithm Explained](https://towardsdatascience.com/simple-reinforcement-learning-q-learning-fcddc4b6fe56)

