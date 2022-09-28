# Banknote-Authentication
Banknote authentication using kmeans clustering

OBJECTIVE
The objective of this data science project is banknote authentication that is to distinguish genuine and forged banknotes. 
THE DATASET
An industrial camera used for print inspection is used here to get the grey scale images of the notes. Then a wavelet transform tool is used to extract the features from the images. The variance and skewness of the wavelet transformed images are the features. And the variance and skewness are plotted on x and y axis respectively. The data type is float64. Here V1 is the variance and V2 is the skewness. The mean of V1 and V2 are 0.433735 and 1.922353 respectively (without normalization) and the standard deviation of V1 and V2 are 2.841726 and 5.866907 respectively (without normalization). Here we have 1372 instances and 2 features. The features are good enough for the dataset that is the number of features is appropriate compared to the instances. The features are useful for analysing the data. The size of the dataset is suitable enough to train the algorithm. Therefore, the dataset can be used for K means clustering.
 
THE PROCESS OF ANALYSIS
The data has been read in csv format. Then the mean and standard deviation of the given data is calculated to analyse the data. The raw data is plotted with V1 and V2 respectively on x and y axis to visualize it. After analysing the features and size of the data, it can be seen that the data is suitable for a Kmeans model. As the aim is to distinguish genuine and fake notes, the data is separated as two clusters by calculating the distance from its centroids. The centroids of the two clusters are marked as black stars. Two different colours have been given to genuine and fake notes that is for the two different clusters.

INTERPRETATION AND ASSUMPTIONS
The given visualization has two variables V1 and V2 showing variance and skewness respectively. Here we have two clusters. The two clusters meet close to zero. The cluster centroids are quite stable with slight variations after running the model 6 times. The black stars represent the cluster centroids. The cluster in the positive side represents genuine notes and the cluster in negative side represent fake notes.
As there is slight variations in the stability of cluster centres there maybe a small percentage of error but the model is reliably accurate.

RECOMMENDATIONS
I recommend to use a more elaborate dataset with good number of instances to train a better model. And Kmeans is a good method to train similar models.

