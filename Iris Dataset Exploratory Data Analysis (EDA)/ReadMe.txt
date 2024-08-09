Iris Dataset Exploratory Data Analysis (EDA)
Overview
This project performs an exploratory data analysis (EDA) on the famous Iris dataset to understand the characteristics and relationships between different iris species. The analysis includes loading the dataset, calculating basic statistics, visualizing the data through various plots, and performing a basic clustering analysis to explore how well the features can separate the species.

Dataset
The Iris dataset is a classic dataset in machine learning and statistics, consisting of 150 samples from three iris species: Iris-setosa, Iris-versicolor, and Iris-virginica. Each species is represented by 50 samples, and each sample has four features:

Sepal Length
Sepal Width
Petal Length
Petal Width
Files
iris_analysis.py: The main script containing all the code for loading the dataset, performing EDA, and visualizing the data.
README.md: This file, providing an overview of the project, steps taken in the analysis, and key findings.
requirements.txt: A list of required Python packages for running the analysis.
Steps of the Analysis
1. Loading the Dataset
The dataset was loaded using Pandas from the UCI Machine Learning Repository.
Basic information about the dataset was displayed, including the first few rows and data types.
2. Data Exploration
Basic statistics such as mean, median, and mode were calculated for numerical columns (sepal length, sepal width, petal length, petal width).
The distribution of each feature was analyzed across the three species.
3. Data Visualization
Histograms and Boxplots: Visualized the distribution of sepal and petal dimensions.
Pairplots: Used Seaborn's pairplot to visualize pairwise relationships between features for each species.
Heatmap: Created a heatmap to visualize the correlation matrix between the features.
Scatter Plot: Plotted the relationship between sepal length and petal length for different species.
4. Advanced Analysis
Violin Plots: Used Seaborn’s violinplot to analyze the distribution of features across different species.
Cluster Analysis: Performed KMeans clustering to see how well the features separate the species without using the species labels. The clustering results were visualized using PCA (Principal Component Analysis).
Key Findings
Species Differentiation:

Iris-setosa is clearly distinguishable from the other two species based on petal dimensions.
Iris-versicolor and Iris-virginica show some overlap, particularly in sepal dimensions, making them harder to distinguish using these features alone.
Correlation Analysis:

Strong positive correlation was found between petal length and petal width.
Sepal dimensions are less correlated with petal dimensions, providing different information for species differentiation.
Clustering:

KMeans clustering identified three clusters corresponding closely to the actual species, with Iris-setosa forming a completely distinct cluster.
Some overlap was observed between Iris-versicolor and Iris-virginica, reflecting the similarities between these species.
Requirements
To run this analysis, you'll need the following Python libraries:

pandas
seaborn
matplotlib
scikit-learn

Conclusion
This project demonstrates the power of exploratory data analysis in understanding and distinguishing between different species in the Iris dataset. By visualizing the data and applying clustering techniques, we can gain insights into how different features contribute to species differentiation and how well unsupervised learning methods can group similar samples.

