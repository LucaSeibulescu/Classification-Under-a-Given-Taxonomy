# VAPRS
## Software Studs Confidence Score Assigner

[Git Repo](https://github.com/SP22-CSCE482/documented-code-github-documentation-varis-vaprs-classifier.git)

Our team created a machine learning model that attempts to detect classification errors of a given product in a hierarchical structure. Retail companies may have thousands of products categorized in a tree-like manner, and this model attempts to detect errors within it.

## Dependencies
In order to run the model, import and install the required dependencies:
- transformers torch
- git+https://github.com/PrithivirajDamodaran/ZSIC.git
- gensim
- nltk
- pickle
- pandas
- numpy
- re
- os
- collections
- operator
- itertools
- string
- csv
- transformers
- sklearn
- PIL

## Code Walkthrough
>The model consists of two main algorithms. 

Firstly, the model strips certain products that contain uncommon labels (i.e. product labels that have classifications in the hierarchy that occur 5% or less) and runs these products through an unsupervised Zero-Shot model. The product’s images and descriptions are parsed and compared to the given labels. A confidence score that a given product matches its label is then output.

Finally, the rest of the products are run through an unsupervised clustering algorithm. Products are parsed of its descriptions, and similarly matched products are bunched together in a cluster, and the model predicts a label name. The confidence score that a given product was classified correctly comes from dividing the amount of correctly labeled products (with respect to the cluster prediction) by the amount of total products in the cluster.


## How to Run
```
Python3 Required
```
1. Pass in a valid dataset. A product dataset should preferably contain a csv file containing a product’s unique identifier, as well as other useful information such as descriptions and item titles. 
2. Pass in a folder containing product images. In addition to that, another separate file should be attached that contains a mapping of product ID’s to the associated images in the product images folder
3. Install required dependencies. See the “Dependencies” section.
Run all cell blocks
4. Receive the outputted CSV file. It should contain all products with the confidence score of each of a product’s classification at a given level in a product taxonomy


