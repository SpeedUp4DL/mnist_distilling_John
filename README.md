# mnist_distilling_John
reproduce 《Distilling the Knowledge in a Neural Network》

## [1] Student Network 
architecture :  two hidden layer , 800 rectified linear unit and no regularization

performance  ： accuracy is 0.9697 on test dataset

source code  ： Student_NN.ipynb

## [2] Teacher Network
architecture :  ConvNets

performance  ： accuracy is 0.9936 on test dataset

source code  ： mnist_distilling.ipynb

weights file ： frozen_model.pb

## [3] Student Distilling Knowledge Network
architecture :  the same to Student Network

performance  ： accuracy is 0.9635 on test dataset

source code  ： Student_Distilling.ipynb

weights file ： frozen_model.pb (teacher model)

super params :  T = 1 （according to paper）， alpha = 0.1 is unkown

when net at a temperture of 20, the performace is very bad and can't converge !!!But I don't know why paper do this?

<p align="center">
<img src="https://github.com/SpeedUp4DL/mnist_distilling_John/blob/master/paper.png" alt="Paper " width="600px">
</p>
