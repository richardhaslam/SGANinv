# Using a GAN-based low-dimensional parameterization to solve inverse problems with complex geologic prior information

This Python 2.7 package contains the (1)spatial generative adversarial network (SGAN) and (2) DREAM<sub>(ZS)</sub> Markov chain Monte Carlo (MCMC) sampler
used for multiple-point statistics simulation and inversion by [Laloy et al. (2018)](https://doi.org/10.1002/2017WR022148)

**Now with a Pytorch 1.1.0 / Python 3.6 GAN-based MCMC inversion example**

## Large data files

Because of Github space limits, the trained SGAN models (needed to reproduce the results presented in the paper) are not provided herein. 
But these are of course available. Please drop me an email if you want to get these files. 

## GAN-based representation

We ported the original 2D SGAN code by Jetchev et al. (2016) to 3D. The codes for training the SGAN with Theano/Lasagne are contained in the SGAN folder. 
Also, 2D and 3D geologic model realizations generated by the trained models can be produced by running the generation2D.py and generation3D.py scripts.

Note that we have a Pytorch 1.1.0 / Python 3.6 version available (see this repo for the GAN-based MCMC inversion and the <gan_for_gradient_based_inv> repo for the training code).

## Performing the inversion

To perform the MCMC inversion within the SGAN latent space using DREAM<sub>(ZS)</sub>, use the run_mcmc.py script from the inversion folder.

## Citation

Laloy, E., Hérault, R., Jacques, D., & Linde, N. (2018). Training-image based geostatistical inversion using a spatial generative adversarial neural network.
Water Resources Research, 54. https://doi.org/10.1002/2017WR022148

## License

The Theano/Lasagne and Pytorch codes for the SGAN are under MIT license while the MCMC inversion code is under GPL license. See the corresponding folders for details.

## Contact

Eric Laloy (elaloy@sckcen.be) 
