#  Tennis Data Regression Analysis 🏸🎾

This analysis uses logistic regression to predict which player is most likely to win the Men's Singles title at the 2025 French Open.

##  Repo Guide 🗂️

- **`atp_files`**: Folder containing all match-level ATP data between 2022 and 2024. This data is sourced from from Jeff Sackmann's [Github repo](https://github.com/JeffSackmann/tennis_atp). 
- **`atp-analysis.ipynb`**: Contains all data cleaning and regression analysis in R.
- **`atp-output.csv`**: Output of the previous file, which will then be used for analysis
- **`atp-output-analysis.ipynb`**: Analysis of how well the model predicts tennis matches and residuals. Also contains analysis for charts.
- **`data`**: Folder containing the csvs that came from the analysis
- **`charts`**: png files of charts used in the story

## Model overview

This analysis uses a regression model with the following features to predict the outcome of a match:
- Difference between two players' elo ratings
- Length of match (best of five vs best of three)
- Surface-level advantage for each player

## Model results

- Statistically significant p-values with a Pseudo R2 of 0.13
- Precision: 66%
- Recall: 66%