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

## Dataset content
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

## Business requirements
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

## Project plan
* Data inspection & cleaning: preparing categorical and numerical features for analysis.
* Descriptive statistics  
* Correlation heatmaps  
* Pairplots  
* Fitness level distributions  
* Visualization: interactive and static plots to present insights clearly.
* Trained classification model predicting fitness level  
* Evaluation metrics: Accuracy, Classification Report, Confusion Matrix  
* Feature importance plot to highlight influential variables
* Dashboards

## The rationale to map the business requirements
To meet the business goal of classifying gym members' fitness levels and uncovering behavioral drivers behind high/low performance, each visualisation was carefully chosen to provide actionable insights for both operational teams (trainers, program managers) and strategic decision-makers.

* Session Duration vs Calories Burned
    Business Need: Identify what contributes to high calorie burn.
    Visual Choice: Correlation plots and trend analysis show that longer session duration is a strong indicator of calorie output. This insight supports creating time-based training goals.
* Experience Level vs Fitness Level / Calories Burned
    Business Need: Understand the impact of training consistency and tenure.
    Visual Choice: Categorical plots (e.g., boxplots, stacked bars) reveal how experience levels correlate with output, aiding coaching program refinement.
* Water Intake vs Fat Percentage & Fitness
    Business Need: Promote health tips that maximize results.
    Visual Choice: Bubble plots and heatmaps highlight hydration’s effect on body composition—informing personalized nutrition plans.
* Workout Frequency and Fitness Level
    Business Need: Encourage consistent training routines.
    Visual Choice: Bar plots and decomposition trees visualize how frequency drives results—supporting gamified loyalty or attendance programs.
* Age vs Calories Burned
    Business Need: Debunk performance myths and support all age groups.
    Visual Choice: Scatterplots and strip plots show that age has minimal influence, supporting inclusive workout strategies.

## Dashboard design


## Analysis techniques used
* Visual Studio Code
* Python
* Jupyter notebook
* ChatGPT
* PowerBI

## Ethical considerations
The dataset is publicly available and contains no private data on individuals.
This project emphasizes ethical AI principles by promoting fairness, transparency, and responsible use of data. All analyses and predictions are designed to support healthier lifestyle choices, not to judge or discriminate. Ensuring privacy, informed consent, and human oversight at every stage fosters trustworthy and accountable AI in the fitness domain.

## Main Data Analysis Libraries
* Pandas
* Numpy
* Plotly
* Seabon
* Matplotlib
* Sklearn
* PowerBI

## Credits

### Resources
* [The Code Institute](https://codeinstitute.net/) Learning Management System
* [VS Code](https://code.visualstudio.com/) was used to write the code
* [ChatGPT](https://chatgpt.com/) was used to generate and debug code
* [README](https://github.com/Code-Institute-Solutions/da-README-template) template
* [Kaggle](https://www.kaggle.com/datasets/valakhorasani/gym-members-exercise-dataset/data) data set was used for this project
* [Logo Image](https://www.gettyimages.de/detail/foto/muscle-network-landscape-blue-lizenzfreies-bild/814346208?adppopup=true)