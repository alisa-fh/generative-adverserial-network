# A Hybrid Adversarial Generative Approach to Generate a White Pegasus
Third year university deep learning summative coursework.

In the Python notebook [here](./pegasus-code.ipynb) we present an implementation and analysis of a deep generative model producing from the CIFAR-10 dataset a diverse set of winged horse images, alternatively known as Pegasi. We specifically use variational autoencoders (VAEs) to leverage the impact of a Generative Adverserial Network (GAN). We replace mean-squared error in VAE with a higher level similarity metric. This is because the element-wise measure used by VAEs do not effectively communicate differences visible to the human eye. A significant pixel-level error would not be as noticable an object transition, for example. By measuring sample similarity with a GAN’s discriminator we train this in conjunction with a VAE. We find this approach produces results superior to a standard VAE when training on birds, airplanes and horses.

Read the methodology, view the VAE-GAN architectures and see results and conclusions in the paper [here](./pegasus-paper.pdf).
