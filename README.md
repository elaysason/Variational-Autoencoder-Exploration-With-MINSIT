# Variational-Autoencoder-Exploration-With-MINSIT
Implementing Variational Autoencoder and explored the importance of each part of its loss function. 


1. [General](#General)
    - [Background](#background)
    - [Program Structure](https://github.com/elaysason/Variational-Autoencoder-Exploration-With-MINST/blob/main/README.md#program-structure)
    - [Running Instructions](https://github.com/elaysason/Variational-Autoencoder-Exploration-With-MINST/blob/main/README.md#running-instructions)
2. [Installation](#installation)
3. [Footnote](#footnote)

## General

### Background
This notbook is  another look into deep learning, this time into Variational-Autoencoders(or VAE in short).VAE is an autoencoder whose encodings distribution is regularised during the training in order to ensure that its latent space has good properties allowing us to generate new images. The VAE in our case while using the MINST data set will generate new number images using the latent variblies learned in the training fase.

![alt text](https://i.imgur.com/TA45raG.png)

### Program Structure
The VariationalAutoencoder is defined containg decoder and encoder using reparametrization trick. The analysis is compased of there main part:
* Evaluting the effect of ![formula](https://render.githubusercontent.com/render/math?math=\{\mu}) on the output by sampling new images from problastic decoder with noisy expectation.
* Evaluting the effect of ![formula](https://render.githubusercontent.com/render/math?math=\{\sigma}) by a performing a similar trial, but this time multipling the std by 0.1,1,10,100
* Looking at the part of each part of the loss function of VAE which is : ![formula](https://render.githubusercontent.com/render/math?math=\{\D_{KL}(q_\phi(z|x)||p_\theta(z))-E_z[logp_\theta(x|z)]}). This is excuted by training only one part at a time.

### Running Instructions
After donwloading the file on colab. Press on file -> open nootbook -> Upload and then drop to downloaded file.

Now you can run the whole nootbok or specfic cells.


## Installation
I will use google as an example but similar procces can be prefomred on other nootbook editors
1. Open google colab
2. Clone the project by:
	```
	!git clone https://github.com/elaysason/Variational-Autoencoder-Exploration-With-MINST.git
	```
<img src="https://i.imgur.com/FNPvWFe.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=30% height=30% />

3. Now the folder is in your files on colab. simpily download the nootbook as showed

<img src="https://i.imgur.com/0FegydE.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=30% height=30% />

