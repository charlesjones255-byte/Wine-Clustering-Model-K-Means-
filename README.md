📌 Project Overview

This project uses unsupervised machine learning to group wines into clusters based on their chemical properties.

Using the K-Means Clustering algorithm, the model identifies hidden patterns in the dataset and groups similar wines together without predefined labels.

🚀 Project Explanation
🔹 What does your model do?

The model analyzes wine features and assigns each sample to a cluster (group) with similar characteristics.

It helps in:

Discovering natural groupings in wine data
Understanding similarities between different wine types
🔹 What algorithm did you use?
K-Means Clustering
Elbow Method to determine optimal number of clusters
🔹 What inputs does the user give?

The user inputs numerical values for:

Alcohol
Malic Acid
Ash
Ash Alkalinity
Magnesium
Total Phenols
Flavanoids
Nonflavanoid Phenols
Proanthocyanins
Color Intensity
Hue
OD280
Proline
🔹 What outputs does the system produce?
A cluster label: 0, 1, or 2
Indicates which group the wine belongs to
🔹 Did you build a UI?

No. The project uses a command-line interface (CLI).

⚠️ Issues Faced
🔹 Overfitting

K-Means does not overfit in the traditional sense, but:

Sensitive to feature scaling
Can produce poor clusters if:
Features have different ranges
Data contains noise/outliers
🔹 Dataset Issues

Dataset sourced from Kaggle:

Challenges:

No labels → difficult to validate results
Possible outliers
Features not normalized
🎯 Project Goal
Learn and apply unsupervised learning
Understand clustering techniques
Build an interactive ML system

📊 Visualizations
📉 Elbow Method

Used to determine optimal number of clusters (K = 3)

📍 Cluster Visualization

Scatter plot showing grouped data points

💾 Model Saving

Model saved using Joblib:

Clustering.pkl

▶️ How to Run
1. Clone Repository
git clone https://github.com/your-username/wine-clustering.git
cd wine-clustering
2. Install Dependencies
pip install -r requirements.txt
3. Run the Model
python model.py

📁 Project Structure
wine-clustering/
│
├── model.py
├── wine-clustering.csv
├── Clustering.pkl
├── README.md
├── requirements.txt
├── app.py   # (Streamlit UI)
🌐 Streamlit Web App (NEW)

Run the web app:

streamlit run app.py

📌 Future Improvements
✅ Add feature scaling (StandardScaler)
✅ Use PCA for visualization
⏳ Add silhouette score
⏳ Deploy online (Streamlit Cloud)

