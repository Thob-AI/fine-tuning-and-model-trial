# OOTDiffusion Fine-Tuning and Inference

This repository contains code for fine-tuning a Stable Diffusion 2.1 model using LoRA (Low-Rank Adaptation) and applying it to virtual try-on tasks with **OOTDiffusion**.

## Project Overview

- **Fine-Tuning:**  
  `sd2_1_fine_tuning with lora.ipynb` — Fine-tunes the Stable Diffusion 2.1 model with LoRA to better adapt to virtual try-on tasks.

- **Inference / Virtual Try-On:**  
  `OOTDiffusion_and SD2.1.ipynb` — Uses the fine-tuned model with the **OOTDiffusion** framework to perform virtual clothing try-ons.

## Files

| File | Description |
|:-----|:------------|
| `sd2_1_fine_tuning with lora.ipynb` | Notebook to fine-tune Stable Diffusion 2.1 using LoRA. |
| `OOTDiffusion_and SD2.1.ipynb` | Notebook to generate virtual try-on results using OOTDiffusion with the fine-tuned model. |

## Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/ootdiffusion-finetuning.git
    cd ootdiffusion-finetuning
    ```

2. **Install dependencies:**

    Make sure you have a Python environment ready. Recommended Python version: `>=3.9`.

    ```bash
    pip install -r ootd_requirements.txt
    pip install -r sd_requirements.txt
    ```

    > **Note:** You may need additional dependencies for OOTDiffusion and Stable Diffusion 2.1 — please refer to their respective setup guides.

3. **Prepare data:**

    - For fine-tuning: Prepare your dataset in the expected format (refer to the notebook instructions).
    - For try-on: Prepare source images and clothing images as per OOTDiffusion requirements.

## Usage

- **Fine-tuning:**

  Open `sd2_1_fine_tuning with lora.ipynb` and follow the steps to fine-tune a pretrained Stable Diffusion 2.1 model.

- **Inference / Virtual Try-On:**

  Open `OOTDiffusion_and SD2.1.ipynb` and run the cells to generate virtual try-on results using the fine-tuned model.

## Acknowledgements

- [Stable Diffusion 2.1](https://github.com/Stability-AI/stablediffusion)
- [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685)
- [OOTDiffusion: Out-Of-The-Box Diffusion Models are Strong Zero-Shot Virtual Try-On Learners](https://arxiv.org/abs/2303.04664)

## Citation

If you use this project or parts of it, please also consider citing [OOTDiffusion](https://github.com/levihsu/OOTDiffusion):

```bibtex
@misc{hsu2023ootdiffusion,
      title={OOTDiffusion: Out-Of-The-Box Diffusion Models are Strong Zero-Shot Virtual Try-On Learners}, 
      author={Hung-Yu Hsu and Yu-Jie Huang and Zi-Yi Ke and Yu-Jie Chen and Chun-Han Lin and Jia-Bin Huang},
      year={2023},
      eprint={2303.04664},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
