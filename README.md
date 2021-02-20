# Capstone Code Repository Table of Contents

Welcome to Capstone Group 4's code repository. Here you can find the code we wrote to build our NBA career success prediction model. 

## Data Acquisition

Note: These data scraping datasets are computationally expensive and require days to complete.

### NCAA 

* [Step 1 NCAA Boxscores](Data_Acquisition/Step1_ncaa_boxscores.ipynb)
* [Step 2 NCAA Player Boxscores](Data_Acquisition/Step2_ncaa_player_boxscores.ipynb)
* [Step 3 NCAA Advanced Boxscores](Data_Acquisition/Step3_ncaa_advanced_boxscores.ipynb)
* [Step 4 NCAA Player Stats](Data_Acquisition/Step4_NCAA_Player_Stats.ipynb)
 

### NBA
* [Step 1 NBA Basic Boxscores](Data_Acquisition/Step1_nba_basic_boxscores.ipynb)
* [Step 2 NBA Player Boxscores](Data_Acquisition/step2_nba_player_boxscores.ipynb)
* [Step 3 NBA Advanced Boxscores](Data_Acquisition/step3_nba_advanced_boxscores.ipynb)
* [Step 4 NBA Player Stats](Data_Acquisition/step4_nba_player_stats.ipynb)
* [Step 5 NBA Draft Scraping](Data_Acquisition/step5_nba_draft_scraping.ipynb)


By the end of this step, you will have successfully completed data scraping and have datasets ready for database loading.

## Data Persistence

### NCAA
* [Step 1 NCAA Boxscores To SQL](Data_Persistence/Step1_NCAA_Boxscores_SQL_Insertion.ipynb)
* [Step 2 NCAA Player Boxscores To SQL](Data_Persistence/Step2_NCAA_Player_Boxscores_SQL_Insertion.ipynb)
* [Step 3 NCAA Advanced Boxscore To SQL](Data_Persistence/Step3_ncaa_advanced_boxscores_sql_insertion.ipynb)
* [Step 4 NCAA Team Schedules To SQL](Data_Persistence/Step4_ncaa_player_career_stats_sql_insertion.ipynb)

### NBA
* [Step 1 NBA Advanced Boxscore to SQL](Data_Persistence/Step1_nba_advanced_boxscores_sql_insertion.ipynb)
* [Step 2 NBA Player Boxscore to SQL](Data_Persistence/Step2_NBA_Player_Career_Stats_ETL_SQL_Insertion.ipynb)
* [Step 3 NBA Player Career Stats to SQL](Data_Persistence/Step3_nba_player_boxscores_sql_insertion.ipynb)
* [Step 4 NBA Draft Data to SQL](Data_Persistence/Step4_nba_draft_data_sql_insertion.ipynb)

### Master Table
* [Player Master Table](Data_Persistence/player_master_table.ipynb)

By the end of this step, you will have all the initial data loaded into our Postgres database.

## Data Exploration

### NCAA 
* [NCAA Box Score Data Exploration](Data_Exploration/ncaa_box_score_data_exploration.ipynb)
* [NCAA Career Statistics Exploration](Data_Exploration/ncaa_career_stats_exploration.ipynb)

### NBA 
* [NBA Simple Box Score Exploration](Data_Exploration/nba_simple_box_exploration.ipynb)
* [NBA Advanced Box Score Exploration](Data_Exploration/nba_advanced_box_data_exploration.ipynb)
* [NBA Player Statistics Exploration](Data_Exploration/nba_player_player_stats_exploration.ipynb)
* [NBA Initial Career Categorization](Data_Exploration/nba_career_categorization.ipynb)


By the end of this step, you will develop an understanding of the trends present in the NBA and NCAA datasets. Note that the both datasets are large but are limited to the year 2000 to present year due to data completeness and availability. 

## Additional Data Acquisition


### High School
* [247 Sports High School Recruiting Data](Additional_Data_Acquisition/247_sports_high_school_data.ipynb)

### NCAA
* [Add NCAA Conference Rank to NCAA player data](Additional_Data_Acquisition/ncaa_aggregation.ipynb)

### NBA 
* [NBA Draft College Renaming List Generation](Additional_Data_Acquisition/nba_draft_college_renaming.ipynb)
* [NBA Draft Rankings Data Scraping](Additional_Data_Acquisition/nba_draft_rankings_scraping_and_sql_insert.ipynb)
* [NBA Composite Score Calculation and Career Clustering](Additional_Data_Acquisition/player_composite_scores.ipynb)

By the end of this step, you will have accumulated three more datasets: high school recruiting data, NCAA strength of conference, and NBA Top 100 Prospect rankings. These datasets will also be loaded into the postgres database that already contains the initial datasets.

## Initial Modeling

* [Active Player Dataset Generation](Initial_Modeling/active_college_players.ipynb)
* [NBA Career Survival Analysis](Initial_Modeling/step1_nba_career_survival_analysis.ipynb)
* [Model 1: NBA Draft Probability](Initial_Modeling/step2_nba_draft_prediction_model.ipynb)
* [Model 2: NBA Career Role Predictions](Initial_Modeling/step3_nba_career_predictions_model.ipynb)


By the end of this step, you will have run through the initial fitting of our modeling efforts. You will have been able to predict which players will be drafted into the NBA. Of those players, the second model you fit will be able to tell you each player's potential NBA career role. 

## Final Modeling

* [Binned Feature Creation on 2020 NBA Draft Class](Final_Modeling/active_player_binned_feature_creation.ipynb)
* [Final Model 1: NBA Draft Probability](Final_Modeling/refit_first_model.ipynb)
* [Final Model 2: NBA Career Role Predictions](Final_Modeling/refit_second_model.ipynb)
* [2020 NBA Draft Class Predictions](Final_Modeling/2020_draft_class_predictions.ipynb)
* [2020 NBA Draft Class Pro Comparisons](Final_Modeling/player_comparisons.ipynb)
* [2020 NBA Draft Class Rankings Generation](Final_Modeling/draft_rankings.ipynb)


By the end of this step, you will have run models to generate predictions on the 2020 NBA Draft class. You will also generate NBA player comparisons for each 2020 NBA draft prospect as well as an overall ranking of the 2020 NBA draft class. 

## Data Story Shiny App

* [Shiny App R Code](../Data_Story/app.R)

The code above generates our shiny app which can be found at https://jpcp73.shinyapps.io/final/. If it is not online, please message Joe Clarkin on Slack for redeployment. 


```python
!tar chvfz notebook.tar.gz *
```

    Additional_Data_Acquisition/
    Additional_Data_Acquisition/.ipynb_checkpoints/
    Additional_Data_Acquisition/.ipynb_checkpoints/247_sports_high_school_data-checkpoint.ipynb
    Additional_Data_Acquisition/.ipynb_checkpoints/nba_draft_college_renaming-checkpoint.ipynb
    Additional_Data_Acquisition/.ipynb_checkpoints/nba_draft_rankings_scraping_and_sql_insert-checkpoint.ipynb
    Additional_Data_Acquisition/.ipynb_checkpoints/ncaa_aggregation-checkpoint.ipynb
    Additional_Data_Acquisition/.ipynb_checkpoints/player_composite_scores-checkpoint.ipynb
    Additional_Data_Acquisition/247_sports_high_school_data.ipynb
    Additional_Data_Acquisition/nba_draft_college_renaming.ipynb
    Additional_Data_Acquisition/nba_draft_rankings_scraping_and_sql_insert.ipynb
    Additional_Data_Acquisition/ncaa_aggregation.ipynb
    Additional_Data_Acquisition/player_composite_scores.ipynb
    Data/
    Data/nba_boxscores.csv
    Data/nba_player_boxscores.csv
    Data/nba_player_boxscores_notebook.csv
    Data/nba_player_career_stats.csv
    Data/ncaa_player_boxscores.csv
    Data/ncaa_player_boxscores_notebook.csv
    Data/ncaa_player_career_stats.csv
    Data/ncaa_simple_boxscores.csv
    Data/247sports.csv
    Data/.ipynb_checkpoints/
    Data/active_players.csv
    Data/2020_season.csv
    Data/binned_data.csv
    Data/test_data.csv
    Data/train_data.csv
    Data/nba_data.csv
    Data/hurdle_model_predictions.csv
    Data/active_binned.csv
    Data/historical_binned.csv
    Data/nba_advanced_boxscores.csv
    Data/nba_team_schedules.csv
    Data/ncaa_advanced_boxscores.csv
    Data/ncaa_team_schedules.csv
    Data/ncaa_team_schedules_etl.csv
    Data/player_career_stats.csv
    Data/staging_player_boxes.csv
    Data_Acquisition/
    Data_Acquisition/Step3_ncaa_advanced_boxscores.ipynb
    Data_Acquisition/step3_nba_advanced_boxscores.ipynb
    Data_Acquisition/.~Step1_nba_basic_boxscores.ipynb
    Data_Acquisition/.~Step1_ncaa_boxscores.ipynb
    Data_Acquisition/Step1_nba_basic_boxscores.ipynb
    Data_Acquisition/Step1_ncaa_boxscores.ipynb
    Data_Acquisition/Step2_ncaa_player_boxscores.ipynb
    Data_Acquisition/step2_nba_player_boxscores.ipynb
    Data_Acquisition/step5_nba_draft_scraping.ipynb
    Data_Acquisition/.ipynb_checkpoints/
    Data_Acquisition/step4_nba_player_stats.ipynb
    Data_Acquisition/Step4_NCAA_Player_Stats.ipynb
    Data_Exploration/
    Data_Exploration/.ipynb_checkpoints/
    Data_Exploration/.ipynb_checkpoints/nba_advanced_box_data_exploration-checkpoint.ipynb
    Data_Exploration/.ipynb_checkpoints/nba_career_categorization-checkpoint.ipynb
    Data_Exploration/.ipynb_checkpoints/nba_player_player_stats_exploration-checkpoint.ipynb
    Data_Exploration/.ipynb_checkpoints/nba_simple_box_exploration-checkpoint.ipynb
    Data_Exploration/.ipynb_checkpoints/ncaa_box_score_data_exploration-checkpoint.ipynb
    Data_Exploration/.ipynb_checkpoints/ncaa_career_stats_exploration-checkpoint.ipynb
    Data_Exploration/nba_advanced_box_data_exploration.ipynb
    Data_Exploration/nba_career_categorization.ipynb
    Data_Exploration/nba_player_player_stats_exploration.ipynb
    Data_Exploration/nba_simple_box_exploration.ipynb
    Data_Exploration/ncaa_box_score_data_exploration.ipynb
    Data_Exploration/ncaa_career_stats_exploration.ipynb
    Data_Persistence/
    Data_Persistence/Step1_NCAA_Boxscores_SQL_Insertion.ipynb
    Data_Persistence/player_master_table.ipynb
    Data_Persistence/.ipynb_checkpoints/
    Data_Persistence/Step1_nba_advanced_boxscores_sql_insertion.ipynb
    Data_Persistence/Step2_NBA_Player_Career_Stats_ETL_SQL_Insertion.ipynb
    Data_Persistence/Step2_NCAA_Player_Boxscores_SQL_Insertion.ipynb
    Data_Persistence/Step3_nba_player_boxscores_sql_insertion.ipynb
    Data_Persistence/Step3_ncaa_advanced_boxscores_sql_insertion.ipynb
    Data_Persistence/Step4_ncaa_player_career_stats_sql_insertion.ipynb
    Data_Persistence/Step4_nba_draft_data_sql_insertion.ipynb
    Final_Modeling/
    Final_Modeling/.ipynb_checkpoints/
    Final_Modeling/.ipynb_checkpoints/2020_draft_class_predictions-checkpoint.ipynb
    Final_Modeling/.ipynb_checkpoints/draft_rankings-checkpoint.ipynb
    Final_Modeling/.ipynb_checkpoints/player_comparisons-checkpoint.ipynb
    Final_Modeling/.ipynb_checkpoints/refit_first_model-checkpoint.ipynb
    Final_Modeling/.ipynb_checkpoints/refit_second_model-checkpoint.ipynb
    Final_Modeling/.ipynb_checkpoints/active_player_binned_feature_creation-checkpoint.ipynb
    Final_Modeling/2020_draft_class_predictions.ipynb
    Final_Modeling/draft_rankings.ipynb
    Final_Modeling/player_comparisons.ipynb
    Final_Modeling/refit_first_model.ipynb
    Final_Modeling/refit_second_model.ipynb
    Final_Modeling/active_player_binned_feature_creation.ipynb
    Initial_Modeling/
    Initial_Modeling/.ipynb_checkpoints/
    Initial_Modeling/.ipynb_checkpoints/active_college_players-checkpoint.ipynb
    Initial_Modeling/.ipynb_checkpoints/step1_nba_career_survival_analysis-checkpoint.ipynb
    Initial_Modeling/.ipynb_checkpoints/step2_nba_draft_prediction_model-checkpoint.ipynb
    Initial_Modeling/.ipynb_checkpoints/step3_nba_career_predictions_model-checkpoint.ipynb
    Initial_Modeling/active_college_players.ipynb
    Initial_Modeling/step1_nba_career_survival_analysis.ipynb
    Initial_Modeling/step2_nba_draft_prediction_model.ipynb
    Initial_Modeling/step3_nba_career_predictions_model.ipynb
    Models/
    Models/nba_model_kbest.pkl
    Models/nba_model.pkl
    Models/second_model_inputs.pkl
    Models/.ipynb_checkpoints/
    Models/nba_career_outlook_model.h5
    ReadMe.ipynb



```python

```
