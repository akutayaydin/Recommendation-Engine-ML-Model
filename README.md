# README

## Overview

This repository contains code for a recommendation system developed for analyzing transactional data and generating personalized recommendations for customers. The system utilizes various techniques, including non-personalized and personalized recommendation methods, as well as market basket analysis.

## Preprocessing

The transactional data is preprocessed to handle missing values and prepare it for analysis:

1. Non-traditional transaction IDs are identified and removed.
2. Missing values in the 'ItemKey' column are filled using the 'Code_Product' column.
3. Redundant columns ('Code_Product' and 'Unnamed: 0') are dropped.

## Recommendation System

### Non-Personalized Recommendations

1. **Popular Items**: Identifies the most popular items based on purchase frequency.
2. **Rating Column**: Assigns ratings to items based on the number of purchases by each customer.
3. **Paired Purchased Items**: Finds frequently purchased item pairs.

### Personalized Recommendations

1. **Matrix Factorization**: Uses Singular Value Decomposition (SVD) to reduce the dimensionality of the customer-item matrix.
2. **Item-Based Collaborative Filtering**: Recommends items to users based on the similarity of their ratings to other users.
3. **Customer-Based Collaborative Filtering**: Recommends products to each customer based on their purchase history and similarity to other customers.
4. **Apriori Algorithm**: Performs market basket analysis to discover frequently bought together items.

## Usage

1. Clone the repository to your local machine.
2. Ensure you have the required dependencies installed (`pandas`, `numpy`, `mlxtend`, etc.).
3. Load your transactional data into the environment.
4. Run the Jupyter notebook or Python script to preprocess the data and generate recommendations.
5. Explore the different recommendation methods and analyze the results.

## Contact

For any questions or feedback regarding the recommendation system or this repository, feel free to contact the repository owner. Your feedback is valuable!
