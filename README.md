# 🌍 Resilient Geo-AI: A Fault-Tolerant Multi-Agent Swarm for Satellite Imagery

> **A deep learning "team" that works together to map the Earth from space, even when sensors fail or environments get harsh.**

---

## 📖 The Story Behind the Project (For Beginners)

### The Problem: The "Single Point of Failure"
Satellites take thousands of pictures of the Earth every day. We use Artificial Intelligence (AI) to look at these pictures and figure out what is on the ground—is it a river, a highway, or a dense forest? 

Usually, scientists rely on **one single AI model** to make this guess. But what happens if the satellite's camera gets blinded by a cloud, or the image gets corrupted by static noise? That single AI model will get confused and confidently give the wrong answer. 

### The Solution: A "Council of Experts"
Instead of relying on one AI, this project builds a **Multi-Agent System**—a team of different AI models working together. 
Imagine a council of three experts looking at a blurry satellite photo:
1. **The Detail Expert (CNN):** Looks closely at local textures, like the sharp edges of buildings.
2. **The Big-Picture Expert (Vision Transformer):** Looks at the entire landscape to see how things connect, like a long river.
3. **The Statistician (Random Forest):** Doesn't look at shapes at all, just mathematically counts the color pixels.

**The Magic:** Because they all "think" differently, they don't make the same mistakes. If a glitch blinds the Detail Expert, the Big-Picture Expert and the Statistician can outvote it. 

---

## 🧠 How the Swarm Works (The Science)

This project doesn't just let the AIs vote; it lets them *negotiate* using advanced mathematics.

* **Opinion Dynamics (The Negotiation):** Instead of a rigid majority vote, the AI agents share their confidence levels with each other and adjust their opinions mathematically until they reach a safe, unified agreement.
* **W-MSR Logic (Ignoring the Crazy Guy):** What if one sensor completely breaks and starts screaming that a grassy field is a highway? We use an algorithm called W-MSR to achieve **Byzantine Fault Tolerance**. Before the AI team makes a final decision, it automatically identifies extreme, outlier opinions and "trims" (ignores) them. The team only listens to the safe, moderate consensus.

---

## 🚀 Key Features & Results

- **Dataset:** Tested on **EuroSAT**, a massive dataset of real Sentinel-2 satellite images covering 10 different types of land (Pastures, Highways, Industrial areas, etc.).
- **Explainable AI (XAI):** We don't just trust the AI blindly. We used "Heatmaps" to look inside the AI's brain. The heatmaps prove the AI is actually looking at the rivers and roads, not just guessing based on background colors.
- **Flawless Recovery:** During testing, we intentionally injected heavy static noise to blind the sensors. While individual AI models crashed and failed, our Multi-Agent Swarm successfully ignored the bad data and stabilized on the correct answer every time.

---

## 📊 Visualizing the Science
*(Note: Upload your project images to your repository and they will appear here!)*

### 1. What the AI "Sees" (Saliency Heatmaps)
*(Shows how our AI accurately targets geographical features)*
![Heatmaps](full_heatmap.jpg)

### 2. Surviving an Attack (Resilience Analysis)
*(The red line shows a single AI failing under noise. The blue line shows our Swarm successfully finding the truth!)*
![Fault Tolerance](Fault_Tolerant_Consensus.png)

---

## 🛠️ Technologies Used
* **Deep Learning:** ResNet-50 (CNN), Vision Transformers (ViT)
* **Machine Learning:** Random Forest
* **Control Theory:** Opinion Dynamics, W-MSR algorithm, Shannon Entropy
* **Geospatial Analysis:** Visible Atmospherically Resistant Index (VARI), EuroSAT

---

## 👨‍💻 Author
**Piyali Dutta** *Capstone Project in AI & Robotics* *Bridging Deep Learning, Remote Sensing, and Decentralized Control Theory.*
