
# Hack.Diversity Data Interview: Product Inclusion Analysis Challenge

## Overview
This technical interview challenge will evaluate your skills in data cleaning, exploratory data analysis (EDA), feature engineering, and predictive modeling within a product inclusion context. Your task is to analyze user engagement with inclusive product features, focusing on accessibility trends and demographic impacts. The final submission should be in the form of a Jupyter Notebook or RMarkdown file, demonstrating your analytical skills and ability to extract insights.

## Objectives
This challenge assesses the following skills:
- **Data Cleaning**: Address missing values and handle outliers in key columns.
- **Exploratory Data Analysis**: Analyze user engagement and feature adoption.
- **Feature Engineering**: Develop new features to enhance your analysis.
- **Predictive Modeling**: Build a basic model to understand user behavior.
- **Visualization Tools**: Utilize tools such as Tableau Public for advanced visualizations, where appropriate.
- **Version Control**: Use GitHub to demonstrate a well-organized, meaningful commit history for each stage of your work.

## Preparation and Setup

1. **Create a New Private Repository**
   - Log in to your GitHub account.
   - Click on the "+" sign in the top-right corner and select **New repository**.
   - Name your repository appropriately (e.g., `HackDiversity-2025-DataChallenge`).
   - Ensure the repository visibility is set to **Private**.

2. **Clone and Push**
   - Clone the original repository to your local machine using the provided link (`git clone` command).
   - Push the cloned content to your newly created private repository.

3. **Add Hack.Diversity as a Collaborator**
   - Navigate to your new private repository on GitHub.
   - Click on the **Settings** tab.
   - In the left menu, select **Collaborators and teams**.
   - Click **Add people** and invite the GitHub account `HackDotDiversity` as a collaborator.

4. **Make Meaningful Commits**
   - Ensure each significant task (e.g., data cleaning, feature engineering, etc.) has its own commit to track progress. Clear, descriptive commit messages will showcase your work methodology effectively.

## Instructions

### 1. Retrieve and Inspect the Dataset
- **Dataset Access**: You have a CSV file containing simulated user interaction data with inclusive product features.
- **Columns**: The dataset includes columns such as:
  - `user_id`: Unique identifier for each user.
  - `feature_used`: Type of feature accessed (e.g., "Colorblind Mode," "Multilingual," "Visual Aid").
  - `session_duration`: Length of the user’s session (in minutes).
  - `engagement_score`: Engagement level on a scale from 1 to 5.
  - `accessibility_settings`: Count of customizations enabled (0-5).
  - `age_group`: Categorizes users by age group.
  - `gender`: Gender (e.g., "Male," "Female," "Non-Binary").
  - `additional_attributes`: Additional user demographics (e.g., "LGBTQ+" or "Person of Color").

### 2. Data Cleaning & Preparation

- **Missing Values**: Identify any missing values and decide how to handle them, especially in `session_duration` and `engagement_score`.
- **Outliers**: Detect and manage outliers in `session_duration` and `engagement_score`.
- **High Accessibility User Classification**: Create a new column called `high_accessibility_user`, classifying users with three or more accessibility settings as a binary label (1/0 or True/False). Explain your choice and its implications for model interpretability.
- **Intersectionality Analysis**: Add a new column that combines `age_group`, `gender`, and `additional_attributes` to facilitate intersectional analysis. For example, label combinations as “Young Adult - Female - Person of Color.”

### 3. Exploratory Data Analysis (EDA)

- **Engagement Score Analysis**: Visualize engagement scores across features and demographics (e.g., age group, gender, additional attributes). Highlight which demographics show the highest engagement for each feature.
- **Feature Usage by Demographic**: Examine patterns in `feature_used` across demographic attributes. Use your new intersectional column to uncover trends that may not appear when demographics are analyzed individually.
- **Recommendation**: Use **Tableau Public** for advanced visualizations such as interactive dashboards, which can provide deeper insights into feature usage and demographic trends. Export key visualizations for inclusion in your final report.

### 4. Feature Engineering & Predictive Modeling

- **New Features**: Create features such as:
  - Average `session_duration` per `feature_used`.
  - Average `engagement_score` by `accessibility_settings` and demographics (e.g., age group, gender).
- **Predictive Model**: Build a simple predictive model (e.g., logistic regression or decision tree) to determine if a user is a `high_accessibility_user`. Use variables such as `age_group`, `gender`, `additional_attributes`, `engagement_score`, and `feature_used`.

### 5. Insights & Recommendations

- **Key Findings Summary**: Summarize insights for each analysis step. Identify which demographics show the most engagement with each accessibility feature.
- **Actionable Recommendations**: Provide data-driven recommendations on how the company can enhance the adoption of inclusive features, particularly among demographics with lower engagement levels.

## Submission Requirements

- **File Format**: Submit a Jupyter Notebook or RMarkdown file containing code, visualizations, and a 3-4 sentence summary for each analysis section.
- **GitHub Submission**: Push your work to GitHub, ensuring a meaningful commit history. Each major section of the analysis should have its own commit, clearly labeled (e.g., “Completed data cleaning” or “Finished EDA”).
- **Google Drive Form Submission**: It is required to submit your final Jupyter Notebook or RMarkdown file through [this link](https://forms.gle/DkpJi7TgLwv2nZLm6).

## Helpful Tips

- **Exploratory Data Analysis**: Use libraries like Matplotlib, Seaborn, ggplot2, or Tableau Public for visualizations.
- **Predictive Model**: Keep it simple with logistic regression or a decision tree.
- **Version Control**: Use clear commit messages for every significant update.

## Evaluation Criteria

Your submission will be evaluated on the following:

- **Data Cleaning & Preparation**: Appropriateness and clarity of data handling.
- **Insights**: Meaningful analysis of trends in inclusive feature adoption.
- **Modeling & Accuracy**: Clarity in model choice and interpretation of results.
- **Presentation**: Clear explanations with supporting visualizations.

Good luck, and showcase your best analysis skills👾!
