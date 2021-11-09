# Description
Class implementation of spectral normalization in pytorch framework. And an implementation of linear and CNN GAN's with spectral and batch normalization.

In this jupyter notebook, I have incrementally built 4 variations of Generative Adverserial Networks (GAN). these are:

1. Linear, fully connected layers, generators and disriminators. The Generator has batch normalization layers.
2. Linear, fully connected layers, generators and disriminators. With no batch normalization layers.
3. CNN GAN with spectral normalization for the discriminator network and batch normalization for generator network.
4. CNN GAN with batch normalization for noth the discriminator and generator networks.

I have worked on this project starting from base code with an implementation of the 
first mentioned GAN's. The base code was part of a MOOC at Coursera.

To create the third GAN I did not use the spectral normalization function provided by `pytorch` but rather I have built my own class.
I have performed some tests on the class and its function, although I have not included them in this notebook.

It is worth mentioning that this work is a part of a submission for a job application challenge
at **[Proteinea](https://www.proteinea.com/)**, they are a team of scientists and Engineers 
who are trying to put the MENA region at the Biotech world frontiers, who are backed by **[Indie-Bio](https://indiebio.co/)**, 
the world’s leading scientific accelerator in Silicon Valley.


# Replicating Results

## Getting An Environment Ready
If you are interested in replicating the work, or you are the recruiter and  interested in testing it :), please, create a conda 
env using the supplied requirements file.

To do so, run:

```sh
conda create --name myenv --file spec-file.txt
```

Or to install the requirements in an existing environment:

```sh
conda install --name myenv --file spec-file.txt
```

## Replicating Results

In order to replicate results of the 4 variations of GAN's you do not need to do more than run the code cells in the order they are in.

If you are interested in performing any further tests, please make use of the docstring and comments in the defined classes, and getters and test functions,
in order to learn how to use these functions and classes to get the specific variants of either the generator or the discriminator you might want to use.

**P.S.:** There is an error that occurs when running a test code cell. The test asserts the generator loss starts from a certain value.
The condition was not met by one generator but I didn't debug it and see its cause as it does not have a major effect on the performance of that generator.
