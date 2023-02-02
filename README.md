# Audio Generation

Under construction

1. Prepare running environment
```
conda create -n audioldm python=3.8
pip3 install audioldm
```

2. Download pretrained checkpoint
```shell
wget https://zenodo.org/record/7600541/files/audioldm-s-full?download=1 -O ckpt/audioldm-s-full.ckpt
```

3. text-to-audio generation
```python
# Test run
python3 scripts/text2sound.py
```

# TODO

- [ ] Update the checkpoint with more training steps.
- [ ] Add text-guided style transfer
- [ ] Add audio super-resolution
- [ ] Add audio inpainting
- [ ] Add AudioCaps finetuned AudioLDM-S model

## Cite this work

If you found this tool useful, please consider citing
```bibtex
@article{liu2023audioldm,
  title={AudioLDM: Text-to-Audio Generation with Latent Diffusion Models},
  author={Liu, Haohe and Chen, Zehua and Yuan, Yi and Mei, Xinhao and Liu, Xubo and Mandic, Danilo and Wang, Wenwu and Plumbley, Mark D},
  journal={arXiv preprint arXiv:2301.12503},
  year={2023}
}
```

## Reference
Part of the code is borrowed from the following repos. We would like to thank the authors of these repos for their contribution. 

> https://github.com/LAION-AI/CLAP

> https://github.com/CompVis/stable-diffusion

> https://github.com/v-iashin/SpecVQGAN 

> https://github.com/toshas/torch-fidelity

# Hardware requirement
- GPU with 8GB of dedicated VRAM
- A system with a 64-bit operating system (Windows 7, 8.1 or 10, Ubuntu 16.04 or later, or macOS 10.13 or later) 16GB or more of system RAM