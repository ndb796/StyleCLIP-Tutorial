### <b>StyleCLIP Tutorial</b>

> This repository provides an unofficial tutorial for StyleCLIP.
* The original paper and source codes can be found in [this link](https://github.com/orpatashnik/StyleCLIP).

### <b>What is CLIP?</b>

* CLIP jointly trains an image encoder and a text encoder using a large dataset.
* An image and text are encoded into similar embeddings if they have similar semantic meanings.

<img width="90%" src="https://user-images.githubusercontent.com/16822641/113474963-ed837300-94ad-11eb-98af-632f4ce4feb9.png"/>

### <b>StyleCLIP Methods</b>

* The StyleCLIP provides three methods based on various previous studies.
* Tutorial: <b>[Lecture note](/StyleCLIP.pdf)</b>
* Tutorial: <b>[Video]</b>

#### <b>Latent Optimization</b>

* A simple approach for leveraging CLIP to guide image manipulation.

<img width="90%" src="https://user-images.githubusercontent.com/16822641/113475055-5e2a8f80-94ae-11eb-8298-2ee1d36e251e.png"/>

* The optimization method requires 200 - 300 iterations that spend several minutes.

<img width="75%" src="https://user-images.githubusercontent.com/16822641/113475177-f58fe280-94ae-11eb-893b-d8d1ba7ef5a3.png"/>

* Google Colab tutorial source code

#### <b>Latent Mapper</b>

* After trained per text prompt (10 hours), the mapper manipulates attributes in one forward pass.

<img width="90%" src="https://user-images.githubusercontent.com/16822641/113475391-64ba0680-94b0-11eb-8183-d2824c8cd674.png"/>

#### <b>Global Directions</b>

* Find global directions in a StyleGAN's style space <b>S</b>.
* After finding a global direction, we can apply this global direction to any latent vector <b>s</b>.

<img width="90%" src="https://user-images.githubusercontent.com/16822641/113475348-05f48d00-94b0-11eb-916b-85ffbffb3b9e.png"/>
