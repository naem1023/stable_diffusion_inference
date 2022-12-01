# Easy Stable Diffusion

Simple and easy stable diffusion inference with LightningModule on GPU, CPU and MPS (Possibly all devices supported by [Lightning](lightning.ai)).

**To install**

```
pip install "sd_inference@git+https://github.com/aniketmaurya/stable_diffusion_inference@main"
```

```python
from stable_diffusion_inference import create_text2image

# text2image = create_text2image("sd1")
# text2image = create_text2image("sd2_high")  # for SD 2.0 with 768 image size
text2image = create_text2image("sd2_base")  # for SD 2.0 with 512 image size

image = text2image("cats in hats", image_size=512, inference_steps=50)
image.save("cats in hats.png")
```
