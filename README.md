# decisin_tree
# 🎬 Decision Tree Movie Classification
This project predicts whether a movie will be a Hit or a Flop using pre-release features such as budget, popularity, vote count, etc. We use the TMDB (The Movie Database) dataset and build a Decision Tree Classifier using scikit-learn.

# 📁 Project Structure
decision-tree-movie-classification/
├── tmdb_movies.csv
├── decision_tree_movie_classifier.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── outputs/
  ├── Decision Tree.png
  ├── confusion-matrix.png
  ├── classification outputs/
    ├── classification-example-output_1.png
    └── classification-example-output_2.png
  └── prediction outputs/
    ├── prediction-example-output_1.png
    └── prediction-example-output_2.png

# 🧠 Model Overview
Model Used: Decision Tree Classifier

Features Used:

Budget

Popularity

Runtime

Vote Average

Vote Count

Release Year

Target: Profitability (1 = Hit, 0 = Flop)

# ⚙️ How to Run
Clone or download the repository.

Open decision_tree_movie_classifier.ipynb in Jupyter Notebook or VS Code.

Install the required libraries listed in requirements.txt.

Run the notebook to see:

Data preprocessing

Model training

Tree visualization

Confusion matrix

Predictions on sample movie data

# ✅ Requirements
Install required packages with:

pip install -r requirements.txt

📊 Sample Outputs
🎯 Decision Tree
Image saved as outputs/Decision Tree.png

📉 Confusion Matrix
Image saved as outputs/confusion-matrix.png

🔎 Example: Movie Classification
movie_index = 123 # Example index from dataset
movie_row = df.loc[movie_index, features]
movie_df = pd.DataFrame([movie_row])
index_prediction = model.predict(movie_df)[0]
print(f"Movie at index {movie_index} is:", "Hit" if index_prediction == 1 else "Flop")

# 📌 Notes
The model only uses pre-release information.

Useful for understanding how early data can help with profitability predictions.

Not intended for commercial use.

# 📄 License
This project is for academic use. Dataset from [TMDB](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).
