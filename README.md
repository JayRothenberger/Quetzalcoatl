## Installation

- Python 3.10.13

  - `conda create -n your_env_name python=3.10.13`

- torch 2.1.1 + cu118
  - `pip install torch==2.1.1 torchvision==0.16.1 torchaudio==2.1.1 --index-url https://download.pytorch.org/whl/cu118`

- Requirements: vim_requirements.txt
  - `pip install -r vim/vim_requirements.txt`

- Install ``causal_conv1d`` and ``mamba``
  - `pip install -e causal_conv1d>=1.1.0`
  - `pip install -e mamba-1p1p1`

## Usage

- `from vim.models_mamba import quetzal_s_patch16_1_24`
- `model = quetzal_s_patch16_1_24()`

## Citation
If you find Vim is useful in your research or applications, please cite it with the following BibTeX entry.

```bibtex
 @article{vim,
  title={Vision Mamba: Efficient Visual Representation Learning with Bidirectional State Space Model},
  author={Lianghui Zhu and Bencheng Liao and Qian Zhang and Xinlong Wang and Wenyu Liu and Xinggang Wang},
  journal={arXiv preprint arXiv:2401.09417},
  year={2024}
}
```

```bibtex
 @misc{weathervim,
  title={Weather Mamba: A Vision Mamba for Atmospheric State},
  author={Jay Rothenberger},
  journal={www.github.com/JayRothenberger},
  year={2024}
}
```
