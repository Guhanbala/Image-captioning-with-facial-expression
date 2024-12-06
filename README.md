
# Image captioning with facial expression

So basicaly what this project does is it produces enhanced captions to the images containing human faces

this project does use pretrained model for emotion detection and image captioning , they where tried to be implemented with available resoureces



## Features

- finds whether the human emotion protrayed is happy or sad
- real time emotion can be deteted
- imgage captioning model done from scartch
- nlp is used to intergrated everything


## Description about our project

the project basically contains 3 sections which 

 a) emotion detection

 b) image captioning model

 c) gpt tool to combine

 ## Emotion detection

 It basically made up of CNN where the real time facial features are extracted and are feeded to distinguish between happy and sad

 ## Image captioning

 the image captioning model is basic encoder decoder structure

 encoder is made up of cnn which is used to extract the the features in the images and made into a feature vector which is feeded as input to the decoder

 decoder is decoder of a transformers which takes the input feature vector and produces captions to the same by producing the coressponding word from the the previous words using softmax

## nlp(gpt 2)
gpt 2 is used to intergtate emotion detected by the cnn and the caption produced for the image and with the extented word limit of 30 
## contributors
i would like to thank 

https://github.com/kamaladhi (Jeevakamal K R)
https://github.com/ShathaVarsha (Shatha Varsha)
https://github.com/GowthamDhanaraju (Gowtham D)

for the remarkable contribution in the project
