# 🇻🇳 Vietnamese Chatbot with LLaMA + RLHF + vLLM

This project showcases the complete workflow for building and serving a Vietnamese large language model (LLM) chatbot. The pipeline includes instruction tuning, reward modeling, reinforcement learning (PPO), and deployment with vLLM.

## 🚀 Project Workflow

1. **Instruction Tuning**  
   - Fine-tune a Vietnamese LLaMA model on instruction-based datasets to teach it how to follow prompts effectively.

2. **Reward Modeling**  
   - File: `[Training]_Reward_Model.ipynb`  
   - Train a reward model to evaluate the quality of generated responses, used later in reinforcement learning.

3. **RLHF (PPO Fine-tuning)**  
   - File: `Train_PPO_Llama_ray.ipynb`  
   - Apply Proximal Policy Optimization (PPO) using Ray to fine-tune the instruction-tuned LLaMA model with feedback from the reward model.

4. **Model Deployment**  
   - File: `Deploy_Vllm.ipynb`  
   - Deploy the final model using [vLLM](https://github.com/vllm-project/vllm), providing an OpenAI-compatible API endpoint with fast inference and streaming support.

5. **Interactive Chatbot UI**  
   - File: `VN_Chatbot.ipynb`  
   - Connects to the vLLM endpoint using the OpenAI SDK and provides a Gradio-based web interface for chatting in Vietnamese.

## 🧩 Tech Stack

- **LLaMA (1B)** – Base language model  
- **Instruction Tuning** – Supervised fine-tuning  
- **Reward Model + PPO** – Reinforcement Learning from Human Feedback  
- **vLLM** – Efficient serving engine  
- **Gradio** – Chatbot interface  
- **Ray** – Scalable training backend  

---

## 🧠 Outcome

A lightweight Vietnamese chatbot built on LLaMA-1B, fine-tuned with both instruction data and RLHF, served via a fast OpenAI-compatible endpoint.

---
