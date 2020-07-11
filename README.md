# Pothole-Detection

## Short Description
A deep learning model is build to detect malaria of the patients with the cell images of the patients.
<br>

# Dataset:
Dataset Link:- <a href="https://www.kaggle.com/atulyakumar98/pothole-detection-dataset</a>
<br>

### 👉 If you like this repo then please give it a ⭐️
<br>

## NOTE:
This project is subject to change by the developer and is still in development
<br>
<br>
<br>
<br>
## To test this out
Testing this is as simple as it gets. Follow this steps:
1. Clone this project.
2. Load the .h5 file in Google Colab
3. Run the following code
```
import numpy as np

from google.colab import files
from keras.preprocessing import image

uploaded=files.upload()

for fn in uploaded.keys():
 
  # predicting images
  path='/content/' + fn
  img=image.load_img(path, target_size=(64, 64))
  
  x=image.img_to_array(img)
  x=np.expand_dims(x, axis=0)
  images = np.vstack([x])
  
  classes = model.predict(images, batch_size=32)
  
  print(classes)
  
  if classes[0]>0:
    print(fn + " is a pathole")
    
  else:
    print(fn + " is a normal")
```
4. When the upload is prompt, choose the image from test_image directory or you can have your own image.
<br>

## Pull Request

Pull Requests are welcome. Please follow these rules for the ease of understanding:
* Make sure to check for available issues before raising one
* Give me a maximum of 24-48 hours to respond
* Have proper documentation on the parts you are changing/adding


## Developed & Maintained by
<br>
<br
[👨 Sayan Nath](https://sayan-nath.web.app/)<br>
[📷 Insta](https://www.instagram.com/sayannath235/)<br>
[🐤 Twitter](https://twitter.com/SayanNa20204009)<br>
[🧳 LinkedIn](https://www.linkedin.com/in/sayan-nath-15a989182/)
<br>
<br>
[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://github.com/sayannath)
