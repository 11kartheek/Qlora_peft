# Qlora_peft

Here is a sample `README.md` file for your GitHub repo:

---

# Fine-tuning PHI 3.5 with QLoRA on OpenAssistant OASST1 Dataset

This repository demonstrates the fine-tuning of the [PHI 3.5](https://huggingface.co/microsoft/Phi-3.5-mini-instruct) model using QLoRA (Quantized Low-Rank Adaptation) on the [OpenAssistant OASST1](https://huggingface.co/datasets/OpenAssistant/oasst1) dataset. The fine-tuning process enables the model to better understand and respond to human-like assistant instructions from the OASST1 dataset.

## About the Dataset

The OpenAssistant OASST1 dataset is a large-scale dataset containing diverse human-annotated conversations, which focus on general instruction following and dialog generation. It is designed to train models to generate human-like responses.

- **Dataset:** [OpenAssistant/oasst1](https://huggingface.co/datasets/OpenAssistant/oasst1)


## Fine-tuning Process

We employ the QLoRA approach to fine-tune the PHI 3.5 model. QLoRA is used to enable efficient fine-tuning by applying low-rank updates to a quantized model, which reduces memory requirements and speeds up training.

### Steps for Fine-tuning

1. **Dataset Loading:** We use the `OpenAssistant/oasst1` dataset to load data and format it for training.
2. **Model Preparation:** The [PHI 3.5](https://huggingface.co/kartheekb7/peft_phi3.5) model is loaded using the PEFT library, and QLoRA is applied to enable memory-efficient fine-tuning.
3. **Fine-tuning:** The model is fine-tuned using the QLoRA method on the instruction-based conversation data.

## Hugging Face Gradio App

You can interact with the fine-tuned model using the Gradio app hosted on Hugging Face. Try the model by providing inputs and receiving conversational responses.

- [Gradio App Link](https://huggingface.co/spaces/Kartheekb7/peft_phi3.5)


