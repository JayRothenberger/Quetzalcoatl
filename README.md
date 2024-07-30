## Installation

- Python 3.10.13

  - `conda create -n your_env_name python=3.10.13`

- torch 2.1.2 + cuda 12.0
  - `pip install torch==2.1.2 torchvision==0.16.1 torchaudio==2.1.1 --index-url https://download.pytorch.org/whl/cu120`

- Per [this](https://github.com/bitsandbytes-foundation/bitsandbytes/issues/212) very helpful issue, to install the neccessary cuda utilities for 
  - `conda install -c "nvidia/label/cuda-12.0" cuda-toolkit`
  then
  - `export export CUDA_HOME=$CONDA_PREFIX`

- Per [this](https://github.com/aws-neuron/aws-neuron-sdk/issues/893) very helful issue, make sure to use the appropriate setuptools version
  - `pip install setuptools==69.5.1`

- Requirements: vim_requirements.txt
  - `pip install -r vim/vim_requirements.txt`

- Install ``causal_conv1d`` and ``mamba``
  - `pip install causal_conv1d>=1.1.0`
  - `pip install mamba-ssm`

- Install ``quetzalcoatl``
  - `pip install -e quetzalcoatl`

## Usage

- `from quetzalcoatl.models import quetzal_s_patch16_1_24`
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
  url={www.github.com/JayRothenberger},
  year={2024}
}
```
