# Sports-Analytics
Analysis of football penalties and predictive model for straight forecast in horse races

## Football Penalties

A dataset of penalties (penalties_dataset_anonymized.csv) is given and we would like to address the following questions:
1. Are the penalty conversion rates between men and women different?
2. Who are the best five penalty takers in the dataset?
3. Develop a order strategy for the penalty shootouts for a team to maximize the probability of winning. Provide a short presentation.

The features of the data are:
- gender: whether this was a men’s or a women’s match;
- competition_id: unique identifier for the competition.
- match_date: the date the match took place.
- match_id: a unique identifier for the match.
- event_type: descriptor for the event. “PG” = penalty goal in normal play; “PM” = penalty
missed in normal play (includes saves as well as off-target shots); “PSM” = penalty missed in a shootout; “PSG” = penalty scored in a shootout.
- home_team_id: the team ID for the team at home in the fixture.
- away_team_id: the team ID for the team who were away in the fixture.
- home_score: the home score before the penalty was taken. This will be set to the score
at the end of extra-time for penalty shootouts.
- away_score: the away score before the penalty was taken. This will be set to the score
at the end of extra-time for penalty shootouts.
- player_id: unique identifier for the player taking the penalty.
- team_id: unique identifier of the team the penalty-taker plays for.
- half: the half of the game the event took place in. 1 = first half of regular time; 2 = second
half of regular time; 3 = first half of extra time; 4 = second half of extra time; 5 = penalty
shootout.
- time: the match time. If an event is in the first half but the time is greater than 45,
assume it is in extra time at the end of the first half. The clock will then reset to 45 for the
start of the second half.
- shootout_order: the order in which penalties were taken in a shootout. Will be NA for
penalties taken during normal play.


## Predictive model for straight forecast in horse races
Given a dataset on horseracing (horse_racing_training_data.csv) to work with, we want to train a model to predict the "Calculated Straight Forecast" price for the holdout set (horse_racing_holdout_data.csv) in a csv file.

The variables of the datasets are:
- race_url: a (made up) URL for the race run;
- X1: The pre race price for the horse that finished 1st;
- X2: The pre race price for the horse that finished 2nd;
- X3: The pre race price for the horse that finished 3rd;
- runners: How many horses were in the race;
- favourite: The price of the pre-race favourite of that race;
- jumps/flat: The type of course the race is on (whether there is fences for the horses to
jump over or not)
- places: number of places being offered in the race
- sf: the straight forecast price (your target variable)
