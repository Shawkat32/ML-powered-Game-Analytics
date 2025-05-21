# ML-powered-Game-Analytics
Project Overview and Objectives
This project focuses on analyzing player performance and behavior in the popular game Fortnite. The objective is to use gameplay data to uncover patterns, group players based on performance, and predict high-performing players using machine learning. Insights gained from the analysis can support game design decisions, enhance player experience, and personalize gameplay feedback. The project also includes a visualization dashboard to help non-technical stakeholders interpret the data effectively.

Technologies Used
Programming Language: Python

Data Visualization: Matplotlib, Seaborn

Machine Learning Libraries: Scikit-learn, NumPy, Pandas

Game Engine: (Data extracted from existing game logs; no engine simulation involved)

Development Environment: Jupyter Notebook


How to Run the Game and Analytics Dashboard
There is no interactive game engine component; the project works with pre-collected gameplay data.

To run the analytics dashboard:

Open the Shorbaj.ipynb Jupyter Notebook.

Run all cells sequentially to:

Clean and prepare the data

Visualize gameplay metrics

Perform clustering and classification

Display results in graphs and tables

The notebook includes all visualization and ML logic in one place for ease of use.

Data Collection Methodology
The dataset, titled "Fortnite Statistics.csv", was compiled from anonymized player sessions. It includes metrics such as:

Eliminations

Accuracy (%)

Damage to Players

Distance Traveled

Damage Taken

These metrics were selected for their relevance in evaluating both combat efficiency and strategic behavior. Data cleaning steps included removing non-numeric characters, handling missing values, and standardizing formats.

Brief Explanation of ML Implementation
Two main machine learning techniques were implemented:

Clustering (KMeans):
Used to identify natural groupings of players based on their stats (e.g., aggressive vs tactical players).
Features used: Eliminations, Accuracy, Damage to Players, Distance Traveled.

Classification (Decision Tree):
Designed to predict whether a player is a “High Performer” (≥3 eliminations).
The classifier was trained on a binary target and evaluated using precision, recall, and F1-score.

Both models were implemented using Scikit-learn and included preprocessing like feature normalization and train/test splits.
