
# 2024 Ballon d'Or Nominees League Stats Dataset

## Introduction

This dataset contains comprehensive statistics for the 2024 Ballon d'Or nominees, collected from various football leagues. 
The data can be used for player performance analysis, comparisons, or machine learning models aimed at predicting player awards 
or other football-related metrics. The dataset includes detailed player statistics, which cover various performance indicators 
such as goals, assists, defensive actions, passing accuracy, and aerial duels won.

## Data Overview

The dataset comprises **237 columns** and **30 rows**, with each row representing a football player. 
Some of the key columns include:
- `league`: The league the player participated in.
- `season`: The season in which the data was collected.
- `team`: The player's team.
- `player`: The player's name.
- Detailed performance metrics such as:
  - **Aerial Duels-Won%**: Percentage of aerial duels won by the player.
  - **Goals Scored**, **Assists**: Offensive contributions by the player.
  - **Defensive metrics**: Including tackles, interceptions, and recovery statistics.

## Files

- `2024 Ballon Dor Nominees League Stats.csv`: This file contains the raw data in CSV format with the following structure:
  - 237 columns representing various player statistics.
  - 30 rows, with each row representing a player.

## How to Use the Data

To use the data in a Python environment, you can load the CSV file with pandas:

```python
import pandas as pd

df = pd.read_csv('2024 Ballon Dor Nominees League Stats.csv')
print(df.head())
```

### Example: Data Analysis

Once loaded, you can perform a wide range of analyses. For example:
- **Compare players**: Compare the performance of two or more players across various metrics.
- **Ranking players**: Rank players based on metrics like goals, assists, or defensive contributions.
- **Model building**: Build predictive models using machine learning libraries like scikit-learn or TensorFlow.

```python
# Example: Ranking players by goals scored
df[['player', 'Goals']].sort_values(by='Goals', ascending=False).head()
```

## Future Enhancements

- Expand the dataset to include more players or historical Ballon d'Or nominees.
- Incorporate additional performance metrics from more leagues or competitions.

This dataset is provided for educational and research purposes only.

