# Brain2GAN

<p>This repo accompanies the paper "Brain2GAN: Feature-disentangled neural coding of visual perception in the primate brain" where we aimed to characterize the high-level neural representations as recorded via cortical implants in a macaque. Our results show that feature-disentangled GAN latents outperform other candidate representations of the visual data in predicting high-level brain activity (i.e., <em>neural encoding</em>). We then used these feature-disentangled representations to reconstruct the perceived stimuli from brain activity with state-of-the-art quality (i.e., <em>neural decoding</em>). You can find our implementations of neural encoding and -decoding in the provided Jupyter notebooks. The brain recordings to achieve these results will be made available upon publication of the paper.</p>



<img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/img.png" alt="stim-recon"/>


### Notebooks

<p>
The following Jupyter notebooks are included in this repository:

<ul>
  <li>`<b>synthesis_faces.ipynb</b>`: This notebook contains the code used to generate the stimulus dataset of face images.</li>
  <li>`<b>synthesis_images.ipynb</b>`: This notebook contains the code used to generate the stimulus dataset of natural images.</li>
  <li>`<b>feature_extraction.ipynb</b>`: This notebook contains the code used to extract intermediate feature activations from VGG16 pretrained on face and object recognition for faces and natural images, respectively, as well as language-regularized CLIP latents.</li>
  <li>`<b>neural_encoding.ipynb</b>`: This notebook contains the code used to predict brain activity from feature representations of recent deep neural networks with different properties such as feature disentanglement and language regularization.</li>
  <li>`<b>neural_decoding_faces.ipynb</b>`: This notebook contains the code used to reconstruct perceived faces from brain activity.</li>
  <li>`<b>neural_decoding_images.ipynb</b>`: This notebook contains the code used to reconstruct perceived natural images from brain activity.</li>
</ul>
</p>

### Time-based neural decoding
<p>The use of intracranial recordings provided for spatiotemporal analysis of brain activity in unprecedented detail. The gifs illustrate how meaningful information gets extracted from the stimulus-evoked brain responses in time. Per trial, neural responses were recorded for 300 ms with stimulus onset at 100 ms. Prior to stimulus onset, the reconstruction is an average-looking image, after which it starts to take on an appearance that closely resembles the originally perceived stimulus.</p>

<table>
    <tr>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0093.png"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0018.png"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0038.png"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0001.png"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/_0094.png"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/_0197.png"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/_0081.png"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/_0114.png"></td>
  </tr>
  <tr>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0093.gif"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0018.gif"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0038.gif"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/0001.gif"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/_0094.gif"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/_0197.gif"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/_0081.gif"></td>
    <td><img src="https://github.com/neuralcodinglab/brain2gan/blob/main/media/_0114.gif"></td>
  </tr>
</table>
