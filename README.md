# VSA_concepts

**Introduction.**
This repository includes all the files developed for the (under review) paper "Vector Symbolic Architectures for semantic features representation". 

Vector Symbolic Architectures are a family of methods that use high-dimensional vectors to represent objects: concepts, trees, sequences, etc. In this work we selected a binary VSA called *Binary Spatter Codes* proposed by Pentti Kanerva. Based on this VSA we designed a model for concept representation that creates "Semantic Pointers" based on a set of semantic features. 

We took the idea of semantic pointers from Eliasmith's model *Semantic Pointer Architecture*. Semantic pointers are vectors used to point to information within a memory system, therefore the term pointer. However, semantic pointers are also 'semantic', which means that the pointers themselves are similar to the information they reference. 

As stated before we create these semantic pointer based on a set of semantic features, which are words that try to define a concept based on its relations with other words. We used the largest semantic feature dataset known in the literature, the McRae dataset. 

**Description of files.**
All codes were implemented as Python Notebooks. This repository also includes the files from the McRae dataset which were slightly modified to acomodate our needs. 

The repository contains two folders: Code and Data. 
Within Code there are three notebooks: Experiments, EncodingDataset and HDComputing_basics.

- **HDComputing_basics** implements all the basic operations to be used with high-dimensional vectors, from generating new random vectors, to operating them. It also contains the description of the clean-up memory as well as its initialization.
- **EncodingDataset** contains all the functions to read the files from the McRae dataset and transform all the concepts and its relations into semantic pointers. 
- **Experiments** uses the functions from the previous notebooks for performing the experiments detailed within the paper.

The only file that needs to be runned to try our codes is Experiments.ipnyb.

**Additional notes**
To successfully try our codes is also needed to download the nltk library, specifically those modules for wordned and wordnet_ic tools. 


