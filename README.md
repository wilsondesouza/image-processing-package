# My Image Processing Package

---

## Description

Image Processing Package is a Python library designed to simplify common image processing tasks. Built on top of scikit-image, this package provides easy-to-use functions for image manipulation, including resizing, histogram transfer, and more.

---

## Features

- Image resizing
- Histogram transfer between images
- Image reading and saving
- Plotting utilities for image visualization

---

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Image Processing Package:

```bash
pip install my-image-processing
```

---

## Usage

Here are some examples of how to use the Image Processing Package:

 ### Resizing Image

 ```python
from image_processing.processing import transformation
from image_processing.utils import io, plot

# Read an image
image = io.read_image('path/to/your/image.jpg')

# Resize the image
resized_image = transformation.resize_image(image, 0.5)

# Plot the result
plot.plot_result(image, resized_image)

# Save the resized image
io.save_image('path/to/save/resized_image.jpg', resized_image)
 ```

 ### Transferring histogram between images

 ```python
from image_processing.processing import combination
from image_processing.utils import io, plot

# Read two images
image1 = io.read_image('path/to/image1.jpg')
image2 = io.read_image('path/to/image2.jpg')

# Transfer histogram from image2 to image1
result = combination.transfer_histogram(image1, image2)

# Plot the result
plot.plot_result(image1, result)

# Save the result
io.save_image('path/to/save/result.jpg', result)
 ```

---

## Acknowledgments

 - This package was built using scikit-image
 - You cant obtain free images from [Pixabay](https://pixabay.com/pt/)

---

## License
[MIT](LICENSE.txt)