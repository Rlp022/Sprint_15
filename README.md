# Sprint_15

# Using Computer Vision for Age Verification in Supermarkets

# Introduction 
Good Seed, a supermarket chain, is exploring the use of Data Science to enhance compliance with alcohol regulations, particularly concerning the sale of alcohol to underage individuals. This project aimed to develop and evaluate a model capable of verifying a person's age from a photograph using computer vision techniques.

# Table of Contents

Project Overview
Exploratory Data Analysis
Model Training and Evaluation
Conclusion

# 1. Project Overview
To ensure a clear understanding of the project goals, an initial quiz was conducted. The primary task involved building a model that could accurately verify a person's age based on photographic data, leveraging computer vision methods.

# 2. Exploratory Data Analysis 
An exploratory data analysis (EDA) was conducted to gain a comprehensive understanding of the dataset. The data included photographs of individuals along with their corresponding ages, which formed the basis for training the age verification model.

# 3. Model Training and Evaluation
Given the computational intensity of the task, model training and evaluation were conducted on a GPU platform. A pre-trained ResNet50 model served as the foundation, with various configurations tested to optimize performance. The results are summarized in the table below:

Dropout	Learning Rate	Test MAE
None	0.0001	6.2608
0.5	0.0001	6.0046
None	0.0005	6.7832
0.5	0.0003	6.8061

# 4. Conclusion 
The most successful model configuration achieved a mean absolute error (MAE) of 6.1 years, which is commendable given the limited size of the dataset. However, despite this progress, a 6.1-year error margin is significant and may not be suitable for age verification in the context of alcohol sales, where precise age determination is crucial to prevent underage sales.

Several challenges were identified, including inconsistencies in image resolution, lighting conditions, face angles, as well as variations in race, gender, and overall image quality. To address these issues, suggestions included standardizing image properties, training separate models for different demographic groups, excluding non-informative pixels, and employing face restoration techniques.

While the project demonstrated the potential of computer vision for age verification, further refinement is needed to ensure the model's reliability in practical applications like supermarket age checks. Nonetheless, this project lays a solid foundation for future work in this domain.
