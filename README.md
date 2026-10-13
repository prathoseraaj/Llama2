# Llama 2 Fine-Tuning

This project fine-tunes the Llama 2 7B chat model using QLoRA and the
`mlabonne/guanaco-llama2-1k` dataset.

## Files

- `fine_tuning_Llama.ipynb` - Training and inference notebook.
- `.gitignore` - Excludes local environments, checkpoints, and model weights.

## Setup

Install the packages used by the notebook:

```bash
pip install torch datasets transformers peft trl bitsandbytes accelerate
```

You also need a Hugging Face account and access to the Llama 2 model.

## Run

1. Log in to Hugging Face:

   ```bash
   huggingface-cli login
   ```

2. Open `fine_tuning_Llama.ipynb`.
3. Run the notebook cells on a CUDA-enabled GPU.

The fine-tuned model is uploaded to:

<https://huggingface.co/prathoseraaj/Llama-2-7b-chat-finetune>

Large model files and temporary training outputs are intentionally excluded
from this GitHub repository.
