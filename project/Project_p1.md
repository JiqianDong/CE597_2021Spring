# CE 597 Project – Part 1 - data preparation  & Homework 1 - Classification

## A. Project Part  1 - data preparation

### A.1 Loading and processing image dataset in python

The data set is ``mnist`` dataset provided in our course git hub website, under the project folder. But in real-world setting, you will probably need to deal with raw data (e.g., ``.JPG`` images). Therefore, the first step of the term project is to load and process raw ``.JPG`` data. You should download the data using the link below

 https://github.com/JiqianDong/CE597_2020s/blob/master/project/dataset.zip

You will find a folder named “training data” after unzipping the file.

There are 10 folders numbered as 0, 1, 2,…, 9 within the training data folder. The number of each folder name is the true label for all the images within that folder. For example, if you look at the images within folder 0, you should find various hand written 0s.

You first task is to write code to successfully load your data, and label them correctly according to the folder name .

For each observation, it should be $(X, y)$, where $X$ is the image data ( $28 \times 28=764$  features representing image pixels), $y$ is the true label (i.e. 0, 1, … ,9).



### A.2 Visualizing data

Here, you need to make sure your data is loaded and process appropriately. Select multiple observations, then print their $y$ and plot the image $X$ using `imshow` function in ``matplotlib`` library.



### A.3 Flatten in to $N \times D$

For training purpose, you have to reshape your dataset into size $N \times D$ where $N$ is the number of images and $D$ is the dimension of features for each image. As mentioned before, $D=28 \times 28=764$, you can use ``np.flatten`` method to flatten a 2D image matrix into a 1D vector.









### A.4 Splitting data

Here, you should split your data into training and validation datasets. 

**Remark**:

Since the original dataset is stored in an ascend order. you have to make sure the training and validation datasets contain all the labels. You can achieve this by first shuffle the overall dataset. Hint: ``np.shuffle``



###  A.5 Saving data as ``.npy`` for future use (Homework #1 and Project – Part 2)

Save your training dataset as well as validation dataset as 4 ``.npy`` file for future use. 

- X_train.npy
- y_train.npy
- X_valid.npy
- y_valid.npy

Make sure you can load them back from these ``.npy`` files.



## B. Homework #1



### B.1  Build classifier with sklearn

For the data prepared in "A. Project Part 1", pick any classifier we discussed in the lecture or class demonstration (e.g., logistic regression, SVM, etc.) and perform the image classification task using ``sklearn`` package in python.



### B.2  Report performance

Train your classifier and  report your model performance in terms of accuracy.  (you will need to further split data for testing as well). Plot a confusion matrix the same as course demo and comment your results.

Submit a short ``.pdf`` report (two pages or less) describing the process and results. Finally, append your code/notebook in the pdf file (this doesn't account for page limit).