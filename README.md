### Drug-Drug Interaction Prediction using Knowledge Graph Embeddings & Conv-LSTM Network
Implementation of our paper titled "Drug-Drug Interaction Prediction Based on Knowledge Graph Embeddings and Convolutional-LSTM Network" submitted The 10th ACM Conference on Bioinformatics, Computational Biology, and Health Informatics(ACM BCB), 2019.

In this paper, we propose a new method for predicting potential DDIs by encompassing over 12,000 drug features from DrugBank, PharmGKB, and KEGG drugs with the help of knowledge graph(KGs). 

In our pipeline, we extract feature vector representation of drugs from the KGs, using various embedding techniques such as RDF2Vec, TransE, KGloVe, SimplE, CrossE, and PyTorch-BigGraph(PBG). The embedded vectors are then used to train different prediction models.

### Requirements
* Python 3
* Keras 
* TensorFlow.

### How to use this repository
  First, collect the DrugBank, KEGG drug, OFFSIDES, and PharmGKB datasets from their website. 
  Then convert them into RDF using 5* linked open data principal e.g. convert the data into n-triple or n-quad format. 
  Then generate the embeddings, which should provide the feature vector for each drug in the knowledge graphs.
  Once you have the feature vectors generated, run the 

### Acknowledgement
The src/ml.py library and RDF2Vec methods are based on https://github.com/rcelebi/GraphEmbedding4DDI by Remzi Celebi et al. 

### Citation request
If you use the code of this repository for your reserch, please consider citing the following paper: 
    @inproceedings{karim2019ddiconvlstm,
        title={Drug-Drug Interaction Prediction Based on Knowledge Graph Embeddings and Convolutional-LSTM Network},
        author={Md. Rezaul Karim, Michael Cochez, Joao Bosco Jares, Mamtaz Uddin, Stefan Decker, and Oya Beyan},
        booktitle={Proceedings of ACM BCB, ACM, New York, NY, USA, 10 pages},
        year={2019}
    }

### Contributing
For any questions, feel free to open an issue or contact at rezaul.karim@rwth-aachen.de
