# Fine-Tuned TinyLlama with LoRA & 8-Bit Quantization

This repository contains code and documentation for fine-tuning the **TinyLlama-1.1B** base model using Parameter-Efficient Fine-Tuning (**PEFT**) and **LoRA** (Low-Rank Adaptation). To optimize GPU memory consumption and accelerate training, the model was quantized to **8-bit** precision using `bitsandbytes`.

The model was trained on the **Awesome-GPT-Prompts** dataset to improve its instruction-following and prompt-generation capabilities.

---

## 🚀 Features

* **Base Model:** `TinyLlama/TinyLlama-1.1B-Chat-v1.0 `
* **Dataset:** `fka/awesome-chatgpt-prompts` (engineered for high-quality persona and prompt generation).
* **PEFT (LoRA):** Efficiently updates a fraction of the parameters, drastically reducing training time and storage footprint.
* **Memory Optimization:** 8-bit quantization (`load_in_8bit=True`) allows training and deployment on budget or consumer-grade GPUs without severe performance degradation.

---

## 🛠️ Installation & Setup

Ensure you have Python 3.10+ and a CUDA-compatible GPU environment. Clone the repository and install the required dependencies:

```bash
git clone [https://github.com/your-username/Fine-Tuned_model.git](https://github.com/your-username/Fine-Tuned_model.git)
cd Fine-Tuned_model
pip install -r requirements.txt
