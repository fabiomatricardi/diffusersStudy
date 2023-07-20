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


 
