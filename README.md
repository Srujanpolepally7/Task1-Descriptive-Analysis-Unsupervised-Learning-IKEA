# Task1-Descriptive-Analysis-Unsupervised-Learning-IKEA
The task1 is to discover some new places here in Sweden that may be suitable for IKEA department stores.By Using the k-means method.


**IKEA DATA: The IKEA dataset contains several columns.**They are

Kommun_code: The IKEA stores consist of different types of code and every
store contains one kommun code
Year : The IKEA data is contains 2010 year data
Kommun_name : The area name of the IKEA store
Revenue : The total revenue of each IKEA store
Employee : The total number of employees in the store
Population : Approximately population store area
Population_University : It's counting population university
Percent_University: Percentage of university.
Productivity : Productivity of percentage.
SalesIndex : Sales index of each IKEA store.
Infrast : The infrast is the basic equipment and structures .
Border : The IKEA dataset contains border only zero's.

**IMPORT LIBRARIES:**

pd : The pd function reads the file.
DataFrame : it creates a dataframe of dataset.
matplotlib : The matplotlib is used for plot visualization.

**DATA EXPLORATION:**

Data exploration is a similar approach to the initial data analysis, whereby a data
analyst users visual exploration to understand what is in
a dataset and the characteristics of the data ,rather than through traditional data
management systems .These characteristics may include data size or quantity, data
completeness,data accuracy ,possible data element relationships.Head: The head is the displays first five records

Tail: The tail displays five bottoms of records.
Info: The info about- the dataset shows the Dtype of each attribute.
Shape: The shape of the dataset.
Describe: The describe contains counts, mean, std, min, 25%, 50%, 75%, max.

**DATA REDUCTION:**

Data reduction is the transformation of empirically or experimentally derived
numerical or alphabetical digital information into a rectified,
ordered, and simplified form. The basic principle is to thea the multitude of data
amounts down to the relevant bits.
Isnull: Isnull syntax identifying missing values of dataframe .
Drop: By using drop syntax is dropping unwanted columns.

**K-MEANS CLUSTERING METHOD:**

Determining number of clusters:
K-means is a form of unsupervised learning, and one of the common methods of
clustering unlabeled data into k clusters.They can also understand how to use the
elbow method as a way to estimate the value k.

**k-means overview:**

before plunging into the dataset let's explore briefly how k-means works:
1: the cycle starts with random initialization of the k centroids.
2:such centroids are used to assign points to his nearest cluster.
3:the mean of all points inside the cluster is used to change the centroids location.
4:The measures above are repeated until centroids values stabilize.

**MinMaxScaler:**

The app scaling is a tool used to standardize the number of independent data
variables or functions.it is also known as data normalization in data processing andis usually done during the preprocessing phase of the data.
Sum_of_squared_distances: The sum of squared distance tends to be zero as k
increases .Imagine that we set k to its maximum value in every sample will form its
own cluster meaning the total of squared distances equals zero.
**ELBOW METHOD:**

If the plot looks like an arm, then the elbow on the arm is optimal k.
In the plot above the elbow is at k=5 indicating the optimal k for this dataset is 5

**SCATTER PLOT OF K-MEANS:**

It shows the number of clusters k through scatter plots.The scatter plots shows with
5 colors bubbles with black bubble indicates.This means of scatter plot is
clustering data of IKEA store data and These many areas of IKEA stores available
in sweden .
**PRINCIPAL COMPONENTS ANALYSIS:**

Principal Component Analysis is a out of a point set in two,tree, or higher
dimensional space, a 'best fit' line can be defined as one that minimizes the average
square distance square distance from one point to the other.The next best fit line
can be chosen similarity from perpendicular to the first direction.Repeating this
process gives an orthogonal basis where different dimensions of the daa are
uncorrelated.

**PERFORM SCALING ON THE DATA:**

first import StandardScalar separate the features from the sales index. 
scale the features PERFORM PCA:

The performs the PCA, the third line loads the principal components into a dataframe.

**COMBINE THE SALES INDEX AND THE PRINCIPLE COMPONENTS:**

The original data comprises nine columns :eight functions and one column of the
revenue index.now for the features we only have two columns after performing PC
and attached back the target column to the new set of principal components.PLOT THE PRINCIPAL COMPONENTS ON 2D:
visualize the new dataset to see how PCA makes it easier to explain the original
data so use scatter plot
Explaining the Variance Using Principal Component:
These values show that the first principal component PC1 explains 54.75% of the
variation in the original data while the second principal component explains
14.04% of the variation in the original data.
