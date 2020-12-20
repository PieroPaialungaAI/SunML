# Convolutional Neural Networks for binary classification of Solar Flares
![sf](https://user-images.githubusercontent.com/55837093/102723811-1b7fe580-430b-11eb-96ce-11be02606321.jpg)



_Hello you! This is my project about Convolutional Neural Networks for binary classification of Solar Flares. If you are interested in the general project and want to know how technology can help astrophysics without any knowledge domain, please go ahead and read chapter 1.\
If you are not interested in the theoretical background of this project, but want to know more about Python, AI and Machine Learning techniques, please skip the first part and move to chapter 2 to discover how to move in the repository and reproduce the compuational experiment.\
If you are interested in both you are just perfect. :) Get an idea of what is the idea of the project in chapter 1, and deepen the computational effort and challenges in chapter 2. 
Welcome aboard,skipper._ 

## 1. About the project

The Sun is the most important star for our planet, as it permits to have life as we know it. One of the most important phenomena of Sun magnetical activity is the one of the  [Solar Flares](https://en.wikipedia.org/wiki/Solar_flare). These are sudden flashes, often seen in the proximity of sunspot and accompanied by enormous energy ejection (coronal mass ejections). Coronal mass ejections can have crucial effects on our lives as radio communication or damage to satellites (or people if we are unlucky) during space missions. The detection and the analysis of solar flares is thus an important task and a necessary effort.\\
Sofisticated techniques have been developed to determine, predict and analyze Solar Flares. Nonetheless the challenge of this GitHub repository is to classify whether or not there is a solar flare in the Sun right now without having any domain knowledge that can cost lot of money and require years of study. 



### 1.1  The Challenge
The challenge of this GitHub Repository is to perform a __binary classification directly on Solar Magnetogram images__, without having no additional information about the Sun magnetic behavior. 
![Screenshot 2020-12-20 at 21 39 46](https://user-images.githubusercontent.com/55837093/102723917-f63fa700-430b-11eb-888a-6dd8104aa8ec.png)

### 1.2  The tool 
The tool that have been used during this process is the one of most powerful algorithm that is called Convolutional Neural Network. \\
This algorithm analyzes each pixel of the image and build a network of parameters that converges to a single number that is the probability of that image to belong to one class. \
In this particular project, two convolutional neural networks have been applied. The __first convolutional neural network__ take the Sun images and detect whether or not there is an active region in the Sun. The __second convolutional network__ take the specific active region portion of the Sun image and detect whether or not there is a Solar Flare in that region or not. 
The first uses the input as a black and white (bidimensional matrix) image. The second one uses the input as a RGB (three-dimensional matrix/tensor) image. 
Anyway they are really similar, and the accuracy is similar too: 
* 94.7% for the first one 
* 95.8% for the second one

## 2. About the code
I'm not going to lie on this one. Data extraction was the most intense job. The development of the CNNs was preatty easy as there are well known structures that do an excellent job in terms of image classification. As we are full of physical information about solar flares it was preatty hard to find raw images of the Solar Flares. An important section of this report is occupied by Web Scraping. 

### 2.1 Software
The language is exclusively Python. __Keras__ libraries were used in order to implement the CNNs, __Pandas__ to data visualization and handling, __matplotlib__ for image data visualization. __PIL__ was used to treat images. __Selenium__ was used to navigate into Chrome with Python. 

### 2.2 "Codes" 
The Codes repository contains horses images. :) \
Just kidding, it has three Jupyter notebooks. The first one is __"activeornot.ipynb"__ and contains both information about the web scraping techniques used to get the active/not active Sun images from [this site] ('ftp://ftp.bbso.njit.edu/pub/archive/2019/') and the Machine Learning CNN part too. In this notebook, the first CNN has been developed.\ As it is, of course, a kind of Supervised Learning, the labels have been obtained by referring to a big page about the Sun that is the wonderful [SpaceWetherLive] (https://www.spaceweatherlive.com/en/solar-activity.html) 
The second notebook is __SFAR.ipynb__ and is 
