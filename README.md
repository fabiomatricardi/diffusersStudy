# diffusersStudy

Studies for python Inferences for image to image generation

---

## Image generation
```
# TEXT-TO-IMAGE CompVis/stable-diffusion-v1-4
client = InferenceClient(token=yourHFtoken)
image = client.text_to_image(prompt="A high tech solarpunk utopia in the Amazon rainforest", 
                             model="CompVis/stable-diffusion-v1-4")
image.save("forest.jpg")
```


## Image to Image generation with API

```
from huggingface_hub import InferenceClient
client = InferenceClient(token=yourHFtoken)
image = client.image_to_image("FELV-cat.jpg", prompt="turn the cat into a tiger", model="timbrooks/instruct-pix2pix")
image.save("tiger.jpg")
```

## Amazing Stable Diffusion Style templates
### Anime style
> strength=0.85, guidance_scale=10

<br>
<img src="https://github.com/fabiomatricardi/diffusersStudy/raw/main/images/singapore12-guidance10.png" height=300>

### Comic art style
> strength=0.85, guidance_scale=10

<br>
<img src="https://github.com/fabiomatricardi/diffusersStudy/raw/main/images/singapore13-guidance10.png" height=300>


### Fantasy art style
> strength=0.85, guidance_scale=10

<br>
<img src="https://github.com/fabiomatricardi/diffusersStudy/raw/main/images/singapore15-fantasyart-guid10.png" height=300>

 
