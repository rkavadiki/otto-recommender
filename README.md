# otto-recommender
Welcome to the codebase for my Otto Recommendation engine, a project submitted to the Kaggle competition.

The notebooks directory comprises the following files, which offer a comprehensive workings of the project.

1. Download_new.ipynb: This script is designed to download the competition files and save them to the data folder, subsequently transcribing the json files into parquet format. Following this, the datasets are segmented into training and validation sets.

2. Covisitation.ipynb: This script is devised to generate three distinct covisitation matrices, thereby indicating which items are simultaneously clicked, added to the cart, or purchased in conjunction. Photographic gravities are assigned based on click, carted, and ordered actions, with further weightage given by factoring in the time between consecutive clicks/orders.

3. Feature_creation.ipynb: This script facilitates the creation of attributes for users, products, and the interrelationship between users and items.

4. Candidate_gen_Ranking.ipynb: This script is used to engender candidates applying covisitation data. Candidates corroborated with the actual click are marked 1 while candidates without any click activity are tagged 0. It constructs an xgboost model and carries out hyperparameter tuning with the hyperopt algorithm.
