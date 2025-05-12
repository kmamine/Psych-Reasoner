# Psych-Reasoner
A multi agent system for mental health simulated therapy, The model learns through reinforcement learning  and adversarial multi agent system. 


# Main Model 
Trained on reasoning and guiding the other party to introspection, shadow work and CBT. 

# Enviroment 
Emulate an env of several personalities of patients with detailed backgrounds behaviours and emotions. With variying levels difficulty, types of mental syndroms, and backgrounds. 

---



# Project Title: Absolute Mental Gym: Multi-Agent Self-Play for Training Introspective Mental Health Agents

**Project Summary**: This project proposes a novel AI training paradigm inspired by the "Absolute Zero Reasoner" to create a highly introspective, psychologically intelligent mental health chatbot. Using a community of diverse synthetic agents that emulate real-world mental health challenges, the system trains via adversarial and cooperative self-play to evolve a central therapist agent capable of nuanced, effective emotional support and guidance grounded in introspection, shadow work, and cognitive behavioral therapy (CBT).


---

1. **Problem Statement**: Current mental health chatbots are either rule-based, limited in depth, or reliant on static datasets. They often fail to:

- Handle complex psychological resistance and trauma.

- Adapt to diverse cultural, emotional, and personality profiles.

- Guide users through introspective or transformative experiences like shadow work.


We aim to address these limitations by creating an autonomous self-play training environment that simulates complex, evolving psychological dynamics.


---

2. Objectives:

- Develop a multi-agent ecosystem of simulated psychological personas.

- Train a central therapist agent via self-play using mental health scenarios.

- Ground responses in introspection, CBT, and Jungian shadow work.

- Enable adversarial, cooperative, and curriculum-based task generation.

- Achieve emotional progress as a measurable, verifiable outcome.



---

3. Core Components:

3.1. Synthetic Agent Community:

- Agents simulate diverse mental health cases with detailed biographies.

- Disorders covered: depression, trauma, anxiety, addiction, etc.

- Variables: cultural background, trauma history, personality traits, belief systems, age, emotional resilience, and resistance.


3.2. Therapist Agent (Target Model):

- Learns adaptive therapy tactics.

- Responds using a blend of introspection, shadow work techniques, and CBT.

- Evolves through reinforcement learning based on emotional and behavioral changes in the agents.


3.3. Self-Play Engine:

- Task proposer agent generates increasingly difficult or novel psychological scenarios.

- Therapist agent attempts resolution.

- Success and failure metrics shape learning.


3.4. Reward System:

- Verifiable emotional progress: reduction in distress markers, increased insight.

- Use NLP to assess sentiment, emotional variance, and acceptance markers.

- Long-term memory change tracking (agents "grow").



---

4. Methodology:

- Use a multi-agent reinforcement learning framework with centralized training.

- Encode psychological profiles into structured memory states.

- Simulate therapy sessions between therapist and synthetic client agents.

- Evaluate outcomes via embedded sentiment/emotion classifiers.



---

5. Technical Stack:

- LLM: LLaMA 3.2, Mistral, or fine-tuned ChatGPT models.

- Frameworks: Langchain, CrewAI for multi-agent orchestration.

- Training: Reinforcement Learning with Self-Play, Curriculum Learning.

- Emotion/Sentiment detection: Fine-tuned RoBERTa/BERT-based models.

- Frontend: Streamlit or React Native (for eventual product).



---

6. Expected Outcomes:

- A benchmark framework for training introspective mental health agents.

- A dataset of adversarial psychological case simulations.

- An LLM-based therapist model capable of navigating resistance and fostering growth.

- An open protocol for emotional progress measurement.



---

7. Feasibility Study:

7.1 Dataset Generation:

- With a well-defined feature composition system (age, trauma history, personality, etc.), we can generate up to ~1 trillion unique persona combinations.

- Each persona will have a profile story (1,000–5,000 words), averaging ~3,900 tokens.

- For 1 billion personas, this amounts to ~3.9 trillion tokens.

- Using DeepSeek or Open Source LLMs for story generation significantly reduces costs versus GPT-4, bringing data generation costs from $39M to ~$10M.


7.2 Model Training Feasibility:

- Training a LLaMA 4-class model (~17B active params) would require upwards of 20–40 trillion tokens for optimal generalization, which aligns with our dataset scale.

- Distributed training infrastructure (TPUs or H100s) is necessary.

- Self-play loops with reinforcement learning can be implemented using RLHF or GRPO-style multi-turn curriculum learning.


7.3 Persona Utility for Self-Play:

- The persona stories serve as the base memory and behavioral script for each synthetic agent.

- Agents act with internal state, memory of their past (auto-regressive), and exhibit reactions to therapy.

- The model learns to track and influence mental/emotional progression over time.


7.4 Optimization Techniques:

- Curriculum learning to begin with simpler cases.

- Use LoRA and quantization to reduce training cost.

- Pre-train with base personas and fine-tune with adversarial multi-turn dialogue.



---

8. Broader Impact:

- Democratize access to affordable, intelligent emotional support.

- Provide a training/testing ground for future therapeutic AI models.

- Empower safe, culturally sensitive mental health AI for global use.



---

Next Steps:

[ ] Define initial personas and disorders for simulation.


[ ] Prototype single-agent vs therapist self-play.


[ ] Build multi-agent orchestration pipeline.


[ ] Define reward functions and evaluation metrics.


[ ] Train and iterate.




