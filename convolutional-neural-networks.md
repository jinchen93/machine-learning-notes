# Convolutional Neural Networks

One use case is to recognize numbers / letters from a picture.

<img src="https://raw.githubusercontent.com/jinchen93/machine-learning-notes/master/diagrams/cnn-inputs.png" alt="CNN Input examples" width="500" />

These are example inputs for the CNN.
These are recognizable for humans, but these inputs are hard for computers to decide.

<img src="https://raw.githubusercontent.com/jinchen93/machine-learning-notes/master/diagrams/decoding-example.png" alt="Example of computer decoding an input" width="500" />

The values are all in different places. So the CNN breaks up the images and matches small patterns instead.

<img src="" alt="Pattern matching" width="500" />

### Filtering

Filtering is when the CNN matches a known pattern to the input patterns.
Each slice is matched against the known pattern and is multiplied by each other.

<img src="" alt="Filtering example" width="500" />

The filter moves around all over the image to see how well that feature is represented.

Convolution is the repeated matching of the filter for all possibilities.

<img src="" alt="Convolution example" width="500" />