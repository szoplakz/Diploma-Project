To use the network the algorithm is split into 3 python projects and multiple files,

Most of the files are there for saving metrics generated and used by the projects

The 40 texts used being in the AlmarimiDocuments Folder
The matching of indices with the 2011 Pan Plagiarism folder can be found using the ALMARIMI-plagiarism matches text document. 

There are 3 projects created found also in the git repository, but they are used in tandem and are not 3 different versions of one another, 
although all of them contain both the Fileparser and the RetinaOperations classes

1. SemanticDetection - this project can be used to extract the semantic fingerprints of individual sentences within the document.
   Originally it was done using the Retina API, but support for it ceased, so now it uses selenium to extract sentences from a still functional demo

2. HTMDetector - uses Python 2.7, unlike the other projects due to the condition of the HTM network implementation not being supported for Python 3,
   Used for training the HTM network, prediction and calculating the anomaly score and likelihood

3. SemanticPlagiarismDetection - Used for everything else, such as other metrics and evaluation and even extracting sentences into files, 
   however requires the fingerprints from 1. and anomaly likelihoods from 2.

Due to git limitations of not uploading files bigger than 25MB, some files had to be compressed and have to be unzipped, they are the following:

partIds.zip and PredictionResults.zip, which unzipped contain their respective characteristics for each individual text

The folders AlmarimiFingerprints and Clean Fingerprints have some of their files zipped individually




The OutputFile text is the final output from the project
