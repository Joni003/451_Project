# 451_Project

#### Eugene Ohba, Jon Karanezi, Clarity Kummer, Max Gehred
___

This project concerns the "MLB Statcast" dataset of all batters in the MLB over the years 2020-2024. This data is made publically avalible by Baseball Savant. To commence the analysis of the "MLB Statcast" dataset, we have imported it into a dataframe, 'df'.

Dataset location : https://baseballsavant.mlb.com/

This dataset `("stats.csv")` consists of 733 observations across 18 attributes. The 18 attributes considered are:
*   last_name, first_name
*   player_id
*   year: year the stats were recorded
*   pa: number of plate appearances
*   k_percent: strikeout rate
*   bb_percent: a walk or (base on balls) rate
*   woba: on-base percentage that accounts for how a player reached a base
*   xwoba: expected weighted on- base average
*   exit_velocity_avg: how hard, on average a batter hits the ball
*   launch_angle_avg: indicates, on average, how often a player hits a fly-ball
*   sweet_spot_percent: how often a player produces a batted-ball event in the launch angle sweet-spot zone of 8-32 degrees
*   barrel_batted_rate: rate at which a player hits a ball with an exit velocity of at least 98 mph
*   hard_hit_percent: percentage of balls batted that were hit at 95 mph or more
*   avg_best_speed:
*   avg_hyper_speed
*   whiff_percent: percentage of swing and misses


The aim of this project is to accurately predict Expected Weighted On-base Average (xWOBA) using 17 predicive attributes. xWOBA is considered to give a comprehensive overview of a player's offensive value. By analyzing the relationships between xWOBA and the 17 other attributes considered, we can gain insights into the most influential aspects of a hitter's performance.

$\textbf{Question of interest:}$

Which features (of those considered in this analysis) are most predicive and significant on a player's offensive value, as measure by Expected Weighted On-base Average (xWOBA)?

$\textbf{Methodologies:}$

A high level overview of the methodolgies we hypothesis will be employed in this project:

*   $\textbf{Data Collection}$: Compile a baseball hitters dataset, made publicly available by MLB Baseball Statcast over the years 2020-2024, ensure representation across a diverse range of players.

*   $\textbf{Data Preprocessing}$: Clean the data for missing values, outliers, and ensure normalization of features when necessary. Additionally, ensure each feature included is relevant to the task at hand.

*   $\textbf{Exploratory Data Analysis (EDA)}$:Visualize the datasets and subsets of such to identify correlations and underlying relationships present within and between attributes. Additionally, analyze the distribution of each feature and the target variable, xWOBA.

*   $\textbf{Feature Engineering}$:Based on EDA findings, engineer new features or transform existing ones.

*   $\textbf{Model Selection}$:Evaluate several regression models, such as Linear Regression, SVM, decision tree, and kNN to deduce which methodology is most appropriate for the dataset at hand.

*   $\textbf{Model Evaluation}:$Use cross-validation to assess model performance, focusing on metrics relevant to regression analysis such as RMSE (Root Mean Squared Error). Additionally, including test, and validation datasets.

*   $\textbf{Feature Importance Analysis}$:Utilize model insights to identify the most influential features in predicting xWOBA, providing valuable insights into hitting performance evaluation.


$\textbf{Expected Outcomes}$ :
A model that accurately predicts xWOBA, identifying features most significant on a player’s offensive value, as quantified by xWOBA.
Strategic insights for players and coaches on improving offensive performance based on model findings.

