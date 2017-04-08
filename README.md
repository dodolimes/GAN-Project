# GAN-Project

This code is taken from https://github.com/jacobgil/keras-dcgan. I have modified the neural network structures in my version of the code.
I have also added a get_dataset() function to pull data from Chars74K set. 

Requirements:
Python 2 or 3
Keras with Tensorflow or Theano backend

To run with Keras using the tensorflow backend, add "image_data_format": "channels_first" to $HOME/.keras/keras.json

I have also added a new argument parser variable "--data". 

To train with MNIST data, run `python dcgan.py --mode train --batch_size <batch_size>`

To train with Chars74K data, run `python dcgan.py --mode train --batch_size <batch_size> --data other`

To generate images run
`python dcgan.py --mode generate --batch_size <batch_size>`
`python dcgan.py --mode generate --batch_size <batch_size> --nice` : top 5% images according to discriminator

To repeat result in the file, run 
`python dcgan.py --mode train --batch_size 128 --data` 
`python dcgan.py --mode generate --batch_size 128 --nice` for MNIST images

`python dcgan.py --mode train --batch_size <batch_size> --data other` 
`python dcgan.py --mode generate --batch_size 128 --nice` for Chars74K images
