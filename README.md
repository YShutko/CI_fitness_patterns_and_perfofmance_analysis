# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

# <div align="center"> Fitness Patterns and Performance Analysis </div>

<p align="center">
  <img src="gettyimages-814346208-612x612.jpg" width="400">
</p>

## Content
* [Readme.md](https://github.com/YShutko/CI_fitness_patterns_and_perfofmance_analysis/blob/b1a86de8fa919e84500b3dfa300965f3f84f622a/README.md)
* [Kanban Project Board](https://github.com/users/YShutko/projects/5)
* [Datasets](https://github.com/YShutko/CI_fitness_patterns_and_perfofmance_analysis/tree/main/data) original and cleaned
* [Jupyter Notebook](https://github.com/YShutko/CI_fitness_patterns_and_perfofmance_analysis/tree/b1a86de8fa919e84500b3dfa300965f3f84f622a/jupyter_notebooks)
* [ML model](https://github.com/YShutko/CI_fitness_patterns_and_perfofmance_analysis/tree/main/model)
* [Plots]()

## Dataset Content
In this project the "Gym Members Exercise Dataset" data set [Kaggle](https://www.kaggle.com/datasets/valakhorasani/gym-members-exercise-dataset/data) is used. 
Dataset cointains the following columns:
* Age: Age of the gym member.
* Gender: Gender of the gym member (Male or Female).
* Weight (kg): Member’s weight in kilograms.
* Height (m): Member’s height in meters.
* Max_BPM: Maximum heart rate (beats per minute) during workout sessions.
* Avg_BPM: Average heart rate during workout sessions.
* Resting_BPM: Heart rate at rest before workout.
* Session_Duration (hours): Duration of each workout session in hours.
* Calories_Burned: Total calories burned during each session.
* Workout_Type: Type of workout performed (e.g., Cardio, Strength, Yoga, HIIT).
* Fat_Percentage: Body fat percentage of the member.
* Water_Intake (liters): Daily water intake during workouts.
* Workout_Frequency (days/week): Number of workout sessions per week.
* Experience_Level: Level of experience, from beginner (1) to expert (3).
* BMI: Body Mass Index, calculated from height and weight.

## Business Requirements
* Understand the key factors that influence individual fitness levels.
* Segment gym members into fitness categories to guide tailored workout plans.
* Use machine learning to automate fitness classification based on physiological and activity data.
* Provide actionable insights for coaches, trainers, and business stakeholders.
* Communicate results clearly using visualizations and dashboards.

## Hypothesis
H1. Higher session duration leads to more calories burned.
Evidence: Strong positive correlation (~0.91) between Session_Duration and Calories_Burned in the correlation heatmap. Clear linear upward trend in the pairplot between these two variables.

H2. More experienced individuals tend to burn more calories.
Evidence: Positive correlation between Experience_Level and Calories_Burned (~0.69). Boxplot shows increasing median calories burned from level 1 → 3.

H3. Water intake is negatively correlated with fat percentage and positively linked with higher fitness level.
Evidence: Heatmap shows negative correlation (~-0.59) between Water_Intake and Fat_Percentage. 
Bubble plot shows more blue (high fitness) points clustering in higher hydration & lower fat% region.

H4. Workout frequency is a strong predictor of fitness level.
Evidence: High positive correlation (~0.84) between Workout_Frequency and Experience_Level, and moderate with Calories_Burned (~0.58). High workout frequency aligns with higher fitness (visible in categorical plots).

H5. Age has little to no impact on calories burned.
Evidence:Heatmap shows weak correlation between Age and Calories_Burned (-0.15). Scatter plot (Age vs Calories Burned) shows no visible trend — points are scattered uniformly.

## Project Plan
* Data inspection & cleaning: preparing categorical and numerical features for analysis.
* Descriptive statistics  
* Correlation heatmaps  
* Pairplots  
* Fitness level distributions  
* Other performance-related insights via plots  
* Trained classification model predicting fitness level  
* Evaluation metrics: Accuracy, Classification Report, Confusion Matrix  
* Feature importance plot to highlight influential variables
* Dashboards

