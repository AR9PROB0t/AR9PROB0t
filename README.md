I make sure you're logged in with 'huggingface-cli login'
from torch import autocast from diffusers import StableDiffusionPipeline
pipe = StableDiffusionPipeline.from_pretrained(
"ComoVis/stable-diffusion=v1-4"
use_auth_token=True
).to ("cuda")
prompt = "a photo of a salad with GPUs"
