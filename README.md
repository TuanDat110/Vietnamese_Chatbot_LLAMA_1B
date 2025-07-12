# Vietnamese Chatbot with LLaMA + RLHF + vLLM

This project demonstrates the full pipeline to build and serve a Vietnamese large language model (LLM) chatbot. The process includes reinforcement learning, reward modeling, deployment, and UI interaction.

## 🚀 Project Workflow

1. **Reward Modeling**  
   - File: `[Training]_Reward_Model.ipynb`  
   - Train a reward model to evaluate response quality, serving as the base for reinforcement learning.

2. **RLHF Fine-tuning**  
   - File: `Train_PPO_Llama_ray.ipynb`  
   - Fine-tune a Vietnamese LLaMA model using PPO (Proximal Policy Optimization) with the help of Ray.

3. **Model Deployment**  
   - File: `Deploy_Vllm.ipynb`  
   - Use vLLM to host the fine-tuned model via OpenAI-compatible API, supporting fast inference and streaming.

4. **Interactive Chatbot**  
   - File: `VN_Chatbot.ipynb`  
   - Connects to the vLLM server using OpenAI SDK and provides a Gradio-based UI for real-time Vietnamese conversation.

## 🧩 Tech Stack

- **LLaMA (1B)** – Base model  
- **RLHF** – Reward-based fine-tuning (PPO)  
- **vLLM** – Fast inference server  
- **Gradio** – Web UI for user interaction  
- **Ray** – Distributed training support  

---

## 🧠 Outcome

An efficient, language-specific chatbot fine-tuned for Vietnamese, capable of being served with OpenAI API compatibility and integrated into any frontend via Gradio.

---

## 🧑‍💻 Author

Created by [Tuan Dat](https://github.com/TuanDat110) • AI Vietnam 2024
