## Why is it bad:
* Leads to misleading metrics and is a common cause of data leaking
* Inconsistencies in labelled data (inclusion/exclusion of detections and bbox sizes)
* Fairly common
	* Even large datasets like CIFAR100 has duplicate images within the train and test sets (4500 found)
## How it can be solved:
* Going over images by similarity, grouping them and removing them such that only 1 image exists within the dataset

Generating embeddings:
* pixel-to-pixel is slow and poor 
* **Embedding**: a vectorization of the information within a source of data
* You can pass an image to a pretrained deep learning model's second last layer to generate an image's embeddings
* Much more efficient
	* Converts millions of pixels to thousands of embeddings

Comparision with cosine_similarity
* can use cosine_similarity(embeddings) to calculate the model
* This provides an NxN matrix for each image to each other image, where diagonal enteries are all 1
	* Subtract by the indentity matrix to ignore these values
* Alternatively: you can batch and parrallel process these embeddings for quicker findings and lower memory usage

Removal:
* thresholding for these values are hit or miss
	* may be able to find that geometric transformations have a 0.94 similarity, colour space transform too, but noise injection might be hard to pin down
* 

(Optional) Uniqueness
* if you have limited resources and want images labelled, you can calculate the set of images that are most unique from the dataset
* Can be done by:
	1. You can use `fiftyone.brain.fob.compute_uniqueness(dataset)`, or 
	2. find the lowest average from calcualating the images' similarties



Resources:
https://towardsdatascience.com/find-and-remove-duplicate-images-in-your-dataset-3e3ec818b978/ (for CIFAR100 and FiftyOne)