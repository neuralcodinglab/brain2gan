# Brain2GAN

This repo accompanies the paper "Brain2GAN; Disentangling neural representations underlying perception in the primate brain via GANs" where we aimed to characterize the high-level neural representations as recorded via cortical implants in a macaque. Our results show that feature-disentangled GAN latents outperform other candidate representations of the visual data in predicting high-level brain activity (i.e., _neural encoding_). We then used these feature-disentangled representations to reconstruct the perceived stimuli from brain activity with state-of-the-art quality (i.e., _neural decoding_). You can find our implementations of neural encoding and -decoding in the provided Jupyter notebooks. The brain recordings to achieve these results will be made available upon publication of the paper.

### Notebooks
The following Jupyter notebooks are included in this repository:

<ul>
  <li>`<b>synthesis_faces.ipynb</b>`: This notebook contains the code used to generate the stimulus dataset of face images.</li>
  <li>`<b>synthesis_images.ipynb</b>`: This notebook contains the code used to generate the stimulus dataset of natural images.</li>
  <li>`<b>feature_extraction.ipynb</b>`: This notebook contains the code used to extract intermediate feature activations from VGG16 pretrained on face and object recognition for faces and natural images, respectively, as well as language-regularized CLIP latents.</li>
  <li>`<b>neural_encoding.ipynb</b>`: This notebook contains the code used to predict brain activity from feature representations of recent deep neural networks with different properties such as feature disentanglement and language regularization.</li>
  <li>`<b>neural_decoding_faces.ipynb</b>`: This notebook contains the code used to reconstruct perceived faces from brain activity.</li>
  <li>`<b>neural_decoding_images.ipynb</b>`: This notebook contains the code used to reconstruct perceived natural images from brain activity.</li>
</ul>

### Time-based reconstruction 

<table>
  <tr>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0093.gif" width="200"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0018.gif" width="200"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0038.gif" width="200"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0001.gif" width="200"></td>
  </tr>
</table>
