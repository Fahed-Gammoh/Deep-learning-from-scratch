# Deep Learning from Scratch

From-scratch PyTorch implementations of CNNs, AlexNet, Vision Transformers, and physics-informed neural networks, with controlled ablations and a shared training framework.

## Projects

| # | Project | Focus | Status |
|---|---------|-------|--------|
| 01 | CIFAR-10 CNN | Baseline, augmentation, regularization | Planned |
| 02 | AlexNet | LRN and dropout ablations | Planned |
| 03 | Hand-built CNN | Conv2d/MaxPool2d as custom autograd functions; depth sweep | Planned |
| 04 | Vision Transformer | From-scratch ViT benchmarked against the CNN | Planned |
| 05 | PINNs | Heat equation and Black–Scholes vs. finite differences | Planned |

## Repository structure

```
shared/      reusable training framework (config, seeding, training loop, checkpointing, logging)
projects/    one folder per project, each with its own README and results
tests/       correctness tests (e.g. gradient checks for custom layers)
```

## Setup

**Local (code and tests):**
```bash
python3.11 -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
```

**Google Colab (training on GPU):**
```python
!git clone https://github.com/Fahed-Gammoh/deep-learning-from-scratch.git
%cd deep-learning-from-scratch
!pip install -e . -q
```

## License

MIT
...
