# ImageNET
An ImageClassifier made using tensorflow's inception-v3

What it does :
It classifies an input image into one of these four categories -- 
                                                                  1) Human Beings

                                                                  2) Plants
                                                                  
                                                                  3) Animals
                                                                  
                                                                  4) Buildings

How to use :
1) Clone the git repository to your local environment.
2) Please ensure that a supported version of python is installed in your pc.
3) Do not disturb the directory structure.
4) Open the command-line tool and go to the cloned directory in your terminal and then execute the following command -
   script/label_image \
   --graph = retrained_model/output_graph.pb --labels = retrained_model/output_labels.txt \
   --output_layer = final_result:0 \
   --image = < Path to Image >
   
   You will get the result as the probabilities of the input image to be of -- 
                                                                               1) Human Beings
   
                                                                               2) Plants
                                                                               
                                                                               3) Animals
                                                                               
                                                                               4) Buildings


How we made :

This is made by retraining the well known tensorflow's image classifier Inception-v3 by removing it's final layer and developing
the output layer based on the training images given divided in the above four categories.

For Documentation, please refer to - https://www.tensorflow.org/tutorials/image_retraining

Training Images are taken from - http://www.image-net.org
