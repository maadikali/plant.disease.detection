# plant.disease.detection


Introduction:

Problem 

Farmers face severe crop loss every year as a result of diseases affecting the plants they grow. 
These problems cause significant financial losses as well as disruptions in the food supply chain. To address these issues, I decided to develop a model that would use photos of plant leaves to determine the condition of the plant. Model will be able to detect diseases and treat them, resolving farmers’ problems in advance.





Literature review with links (another solutions) 
In general, the project is based on Assignment 2, which includes a github link, as well as a tutorial and dataset from Kaggle.
Plant Leaf Disease Detection with GUI | ML Projects | Machine Learning Training (morioh.com)
deep-learning-with-python-notebooks/5.2-using-convnets-with-small-datasets.ipynb at master · fchollet/deep-learning-with-python-notebooks · GitHub
Assignment 2 
Plant Village | Kaggle
Image classification  |  TensorFlow Core


Current work (description of the work)

My model takes an image as input and predicts whether or not it has a disease before classifying it to a specific type of disease. 
The dataset is divided into three parts: training, which contains 60% of the images, validation, and test, which each contain 20%.

Github link: https://github.com/maadikali/plant.disease.detection/tree/master

YouTube link: Plant Disease Detector - YouTube



Data and Methods

Information about the data (probably analysis of the data with some visualisations)

Overall, my dataset includes more than 200 images of leaves that are either classified as healthy or diseased, for example below is a tomato leaf
that has bacterial disease and a healthy potato leaf. 


![photo_2023-02-19_18-31-01](https://user-images.githubusercontent.com/97117948/219948105-f58f81d6-a134-4225-8cae-bae141bb8252.jpg)



Description of the ML models you used with some theory 

It is made up of Conv2D layers, which use convolutional filters to extract features from input images, 
MaxPooling2D layers, which prevent overfitting by providing an abstract form form of the representation, 
and Flatten layers, which convert the results of the convolutional layers into a 1D vector, which is then passed to the Dense layers for classification.

Results 
 Results with tables, pictures and interesting numbers

![photo_2023-02-19_18-31-11](https://user-images.githubusercontent.com/97117948/219948178-93656595-5e2b-4d7f-8e89-9aa418173872.jpg)





Here is the statistics for the model: 
By each training accuracy reached 99% and loss dropped below 5%


![photo_2023-02-19_18-31-22](https://user-images.githubusercontent.com/97117948/219948208-bb94e8d0-cf91-4bf9-a91d-5ad8fcc6d5d1.jpg)




The screenshot below shows that the model has a high accuracy rate in all cases.

![photo_2023-02-19_18-31-33](https://user-images.githubusercontent.com/97117948/219948227-e2b14178-2f2b-480a-9a1f-94b611305d77.jpg)



Discussion 
Critical review of results 

Here are the results of a model based on images, as you can see in all cases it predicted the plant's condition flawlessly.
However, it’s limited only by particular types of diseases from the database, meaning that disease coverage is low. 
Unfortunately, my laptop is not powerful enough to include more disease types and for that reason I have chosen only widespread diseases.
This project can further be improved by scaling the dataset, deploying the website on a server and creating convenient User Interface 
for good interaction with users. 


![photo_2023-02-19_18-31-40](https://user-images.githubusercontent.com/97117948/219948238-91624ac9-1f3d-40a6-a2d0-9ddc8cf7c3ea.jpg)
