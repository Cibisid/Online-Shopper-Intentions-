🛍️ Online Shoppers Clustering using Machine Learning
This project applies unsupervised learning techniques to cluster online shoppers based on session behavior and demographic features. The clusters are evaluated using the Rand Index (RI) against actual purchase behavior (Revenue), to assess how well the clustering models group similar shoppers.

📊 Project Overview
Clustering Algorithms Used:

K-Means Clustering

Agglomerative Clustering (Complete-Linkage)

Goal: Group similar online shoppers and evaluate clustering performance using Rand Index (RI) against actual purchase outcomes.

🗂 Dataset
File: online_shoppers_intention.csv

Format: CSV

Source: E-commerce user session logs

Evaluation Label: Revenue (binary: True / False)

🛠 Installation and Dependencies
Make sure the following libraries are installed:

pip install pandas numpy scikit-learn matplotlib
Required Libraries:

pandas

numpy

scikit-learn

matplotlib

🔄 Data Preprocessing
One-hot encoded categorical columns

Handled missing values

Standardized numeric features using StandardScaler

No train/test split — clustering is performed on the entire dataset

Converted Revenue to binary numeric format for evaluation

🤖 Clustering & Evaluation
🔹 K-Means Clustering
Clusters: 4

Initialization: Random, random_state=42

🔸 Agglomerative Clustering
Clusters: 4

Linkage: Complete

Distance Metric: Euclidean

📏 Evaluation with Rand Index (RI)
Custom rand_index() function implemented

RI compares predicted cluster assignments to actual purchase labels (Revenue)

Measures pairwise agreement between true and predicted labels

✅ Results
Model	Rand Index
K-Means	0.5792
Agglomerative	0.7377
Best Model	✅ K-Means Clustering (based on evaluation criteria)
Although Agglomerative Clustering had a higher RI score, the final selection may depend on additional interpretability and performance metrics discussed in the notebook.

▶️ How to Run
Open the .ipynb notebook in Google Colab

Upload the dataset online_shoppers_intention.csv when prompted

Run all cells:
Runtime > Run all

View the Rand Index scores and the best-performing model in the output

📝 Notes
Ensure the correct CSV file is uploaded

Results may vary slightly without a fixed random_state

No train/test split was performed—clustering used the full dataset

👤 Author
Cibi Siddarth
University of North Florida
School of Computing
