# CSI4107 Data Retrieval - Assignment 1 - Group 12

### Assignment Reference
https://www.site.uottawa.ca/~diana/csi4107/A1_2023.htm
## Group 12 Members & Contribution:
* Simon Proulx 300067852 - Part of Step 1 & general project organization (github, report file, etc.)
* Manav Patel 300074687 - Part of Step 1 & Step 2
* Mahdi Chiboub 300094626 - Step 3 in its entirety

## Setting Up
Prerequisites:

1.  `python3` installed and executable.
2.  `nltk` libaries installed (all of these can be downloaded using `python3` -> `import nltk` -> `nltk.download('corpus | tokenize | stem.porter')`
3. `Beautifulsoup bs4`

## Program Functionality
to run the program, simply run main.py in your preferred python environment. Each step will be ran in their respective .py program: 
`1.` preprocess.py
`2.` Indexer.py
`3.` RankerAndRetriever.py

## Functionality
The Assignment's task was to implement an Information Retrieval System for a collection of documents, similarly formatted to .xml files. The steps are as follows:
1.  the Preprocessor finds all elements of "text" within the files, identifying the textboxes in the folder. it will then tokenize each word in the dictionary. The dictionary is saved as a .jason and used in step 2.
2. The indexer will use the tokenized dictionary to identify the weight of each word in the collection. it will do this process using the word frequency in the collection. Through this process, it will create an inverted index.
3. Finally, compute the cosine similarity scores in the inverted index between each document. This will identify the topics that are most similar between eachother.

## Algorithms, Data Structures & Optimizations

The preprocessor takes the original folder and compiles it into a .json dictionary. We used BeautifulSoup as a library that easily identifies the parts of the documents which are in textboxes. This is because bs4 is an xml parser, which allows us to parse eloquently. For stopwords and punctuation, we merely use nltk library to remove it. 

## Vocabulary & Tokens

## Mean Average Precision Score (trec_eval)

## Results
