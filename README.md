<div align="center">

<pre>
███╗   ███╗██╗     ███╗   ██╗ ██████╗ ████████╗███████╗███████╗
████╗ ████║██║     ████╗  ██║██╔═══██╗╚══██╔══╝██╔════╝██╔════╝
██╔████╔██║██║     ██╔██╗ ██║██║   ██║   ██║   █████╗  ███████╗
██║╚██╔╝██║██║     ██║╚██╗██║██║   ██║   ██║   ██╔══╝  ╚════██║
██║ ╚═╝ ██║███████╗██║ ╚████║╚██████╔╝   ██║   ███████╗███████║
╚═╝     ╚═╝╚══════╝╚═╝  ╚═══╝ ╚═════╝    ╚═╝   ╚══════╝╚══════╝
</pre>

### Hand-rolled ML notebooks — PyTorch + math + experiments

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.x-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](./LICENSE)

</div>

Two parallel collections of 48 notebooks each — **English** (`en/`) and **Brazilian Portuguese** (`pt/`) — written from scratch with my own commentary, LaTeX derivations and runnable PyTorch experiments. Every notebook is self-contained: intuition → math → implementation → experiment → discussion.

## Categories

| # | English | Portuguese | Topics |
|---|---------|------------|--------|
| 01 | `en/01_pytorch_basics` | `pt/01_fundamentos_pytorch` | hello-world, gentle intro, computational graphs, MLP from scratch, first NN |
| 02 | `en/02_classical_ml` | `pt/02_ml_classico` | linear / logistic regression (from scratch + concise) |
| 03 | `en/03_nlp_basics` | `pt/03_nlp_basico` | bag of words (+ DataLoader), CBOW, Deep CBOW |
| 04 | `en/04_language_models` | `pt/04_modelos_de_linguagem` | log-linear LM (+ DataLoader), neural LM (+ batched) |
| 05 | `en/05_transformers` | `pt/05_transformers` | scaled dot-product attention, multi-head, positional encoding, encoder, decoder (mini-GPT), BERT fine-tuning, LoRA, KV-cache, tokenisers, RoPE, MoE |
| 06 | `en/06_graph_neural_nets` | `pt/06_redes_neurais_grafos` | intro GNN (PyG), GCN from scratch, GAT |
| 07 | `en/07_math_foundations` | `pt/07_fundamentos_matematica` | linear algebra essentials, mean / variance, feature scaling |
| 08 | `en/08_diffusion` | `pt/08_difusao` | DDPM on MNIST, score matching, classifier-free guidance |
| 09 | `en/09_rl` | `pt/09_aprendizado_por_reforco` | REINFORCE, DQN, PPO |
| 10 | `en/10_optimization` | `pt/10_otimizacao` | SGD vs Adam, Lion, LR schedules |
| 11 | `en/11_interpretability` | `pt/11_interpretabilidade` | Integrated Gradients (Captum), attention rollout, Grad-CAM |
| 12 | `en/12_efficient_training` | `pt/12_treinamento_eficiente` | mixed precision (AMP), gradient checkpointing, `torch.compile` |

## Notebook structure

Every notebook follows the same template:

1. **Title + series header** linking back here.
2. **Intuition** — short prose explanation of what we're solving and why.
3. **Mathematical formulation** — LaTeX, numbered when useful.
4. **Implementation** — PyTorch (and NumPy where relevant).
5. **Experiment** — small dataset, plot, numbers.
6. **Discussion** — limitations, gotchas, modern variants.
7. **References** — pointer to this repo + author profile.

## Running

```bash
# Minimal setup
python -m venv .venv && source .venv/bin/activate
pip install jupyter torch torchvision matplotlib numpy

# Topic-specific extras (install per notebook)
pip install transformers datasets accelerate     # transformers / BERT
pip install captum                                # interpretability
pip install gymnasium box2d-py                    # RL
pip install torch-geometric                       # GNN

jupyter notebook
```

Pick a category, open a notebook, run cells top-to-bottom.

## License

MIT — see [`LICENSE`](./LICENSE).

## Author

Fernando Bezerra — [@Nandobez](https://github.com/Nandobez)
