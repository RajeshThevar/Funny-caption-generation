# Funny-caption-generator-NLP
A deep learning NLP model to auto generate funny captions for the new york caption contest for cartoon images.

Goal is to see if we can generate funny natural language sentences. And New York caption contest gave us the right dataset/tools. This idea went onto see if we can generate funny captions relevant to a given cartoon image. 

Okay, this model is trained on both images and previous user submitted captions to the New York caption contest; so this is achieved through deep learning and word2vec embeddings. The deep learning model contains two parallel networks as shown in this below image. One network is convolutional neural network, pre-trained VGGnet CNN model. You see, there aren't "any" models trained on identifying cartoon image characteristics, or there aren't much single pattern cartoon images. Example, a cat can be drawn in multitude of ways. 
      But every images are just numbers, and we have only 30 cartoon images from the contest dataset. What I have did here is just extract numbers (features) from different cartoon images. Each cartoon image from 30 gives different feature even though we had used CNN and VGGnet to extract features from cartoon images. 
      
Main goal is to generate funny captions. So we have used LSTM neural networks and built a language model to generate new funny (experimented) captions. 
      But we do have to generate sentences related to given cartoon image right? So we have used a merge architecture method to combine both extracted features, both neural networks in tandem, from dataset and get trained on. To later generate captions relevant (somewhat) to given cartoon image. Trained model will act like describing what is in the image. Can be used to such tasks as well. Here is a peek into the results anyway.
      
 Dataset of the New York humor caption contest is from: https://github.com/nextml/caption-contest-data
 Load model file: https://www.dropbox.com/s/jx5qubg6cahtq48/last_resort.h5?dl=0

  ![alt text](https://github.com/RajeshThevar/Funny-caption-generation/blob/master/Architecture.png)
  ![alt text](https://github.com/RajeshThevar/Funny-caption-generation/blob/master/Example%20cation%20generated%20for%20this%20cartoon%20image.png)
  ![alt text](https://github.com/RajeshThevar/Funny-caption-generation/blob/master/example%20caption%20generated%20by%20machine%20model%20for%20this%20cartoon.png)
  ![alt text](https://github.com/RajeshThevar/Funny-caption-generation/blob/master/examply%20funny%20caption%20generated.png)
  ![alt text](https://github.com/RajeshThevar/Funny-caption-generation/blob/master/Example%20caption%20generated.png)
