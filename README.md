# Semantic-Similarity-Arabic
This is a Class meant for specific functionality with Arabic Large Language Models. The class only uses two metric for Semantic Similarity, Cosine
Similarity and Euclidean Distance (for now). It is only meant to be used with transformers that return PyTorch objects. I intend on updating this to
work with TensorFlow objects as well. 
Pre-processing is done using the Camel-Tools library.
This classes uses the Faiss library for optimization of comparison for encoded sentences. I will update this to have detailed descriptions
of the models, math, and algorithms - for now, you can consult their library documentation for more details.

How to use: First clone this repository using this line 


`git clone https://github.com/FDSRashid/Semantic-Similarity-Arabic.git`


Then, move into the newly cloned repository using 

`cd Semantic-Similarity-Arabic/`

Next, install using  the following line: 

  
  `pip install .`

  
  The install will take a few minutes. Finally, you can import a module that uses a specific metric by importing from its respectively named folder. this example code loads the CosineSimilarity class:    
  
  `from cosinesimilarity.cosine_similarity import CosineSimilarity` .  
  
Unless updated in future versions, this is how all metrics I implement will be named and organized.

For a list of functions most useful to the user, navigate to the 'semanticsimilarityarabic' folder and click on the semanticarabicsimilarity.py file. In there, I've listed the functions that all the Classes must implement. These will be the most useful functions for the user. Each Class implementation has its own set of functions useful for implementing its version. Explore if you'd like!

Important Node: I am intending to implement a class that requires datasets from camel_tools. As of the latest update, Cosine Similarity and Euclidean Distance Classes will not require these datasets. However, to implement jaccard similarity, i am using their models specifically to tokenize arabic words and split words into suffixes and prefixes as well. I've linked their github on instructions to download their data sets. Please follow their instructions strictly - issues that come from the jaccard class 
pertaining to downloading the dataset I can't help with. Note there is different insructions for using the dataset on desktop and on google colab. : https://github.com/CAMeL-Lab/camel_tools#installing-data 

Author : Ferdaws Rashid


Email: frashid@berkeley.edu
