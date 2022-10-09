# Datasheet Template

As far as you can, complete the model datasheet. If you have got the data from the internet, you may not have all the information you need, but make sure you include all the information you do have. 

## Motivation

- For what purpose was the dataset created? 
The MNIST dataset is a large database of handwritten digits that is widely used for the training and improvement of image processing systems.

- Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?
The MNIST dataset was created by the National Institute of Standards and Technology (NIST). This is a physical sciences laboratory and non-regulatory agency of the United States Department of Commerce. The MNIST database was created originally in 1998 as a combination of two of NIST's databases: Special Database 1 and Special Database 3. These databases consist of digits written by high school students and employees of the US Census Bureau.

 
## Composition

- What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)? 
The instances comprises an image and its label.

- How many instances of each type are there? 
The MNIST Dataset consists of 70k 28x28 pixel grayscale images of handwritten digits extracted from two NIST databases. The training set consists of 60,000 images, and the test set comprises 10,000 images. There is one digit per class with a total of 10 classes (0-9), with 7,000 images in each class. 

- Is there any missing data?
Not that I am aware of.

- Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?
No the data is entirely public information and is widely accessible.

## Collection process

- How was the data acquired? 
The data was acquired using the DataLoader method using PyTorch

- If the data is a sample of a larger subset, what was the sampling strategy? 
I don't think the data is part of a larger subset.

- Over what time frame was the data collected?

## Preprocessing/cleaning/labelling

- Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section. 
For this project, the data had already been pre-processed, and there was no requirement for me to clean/label any of the data.

- Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?
The data is saved online 
 
## Uses

- What other tasks could the dataset be used for? 
The MNIST dataset has been effectively solved multiple times. However, it remains a very useful dataset as a starting point for developing image solving convolutional neural networks.

- Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms? 

- Are there tasks for which the dataset should not be used? If so, please provide a description.
The data is only grayscale images, therefore it should not be used to test CNNs that are seeking to classify images with more than 1 channel input. 

## Distribution

- How has the dataset already been distributed? 
The dataset is free to download through a wide number distributors. For example, Kaggle has a csv file available to download. Tensor formatted versions are available through PyTorch.

- Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?  
No
## Maintenance

- Who maintains the dataset?
The National Institute of Standards and Technology maintain the dataset. The dataset curators are listed as Chris Burges, Corinna Cortes, and Yann LeCun

