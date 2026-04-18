# Pitch-Quality-Modeling-with-Random-Forest-XGBoost
Overview
This project builds two predictive models to estimate the run value of individual pitches using Statcast data. The goal was to predict run_value — a measure of how much a pitch contributed to run scoring — using pitch characteristics and game context.
Models
RF_STUFF — Random Forest (ranger)
Uses pitch type, velocity, horizontal and vertical break, plate location, home team, and batter handedness.
BETTER_STUFF — XGBoost
Uses velocity, horizontal and vertical break, plate location, spin rate, balls, and strikes. Slightly outperformed the Random Forest baseline.
Results
RF_STUFF (Random Forest)~0.049 BETTER_STUFF (XGBoost)~0.045
BETTER_STUFF outperformed the course benchmark Random Forest model.
Tools & Packages

R, tidyverse, ranger, xgboost, caret, Metrics

Variables Used: RF_STUFF (Random Forest):

pitch_type
release_speed
pfx_x
pfx_z
plate_x
plate_z
home_team
stand

BETTER_STUFF (XGBoost):

release_speed
pfx_x
pfx_z
plate_x
plate_z
release_spin_rate
balls
strikes
