# Personalized Student Recommendations

## Overview
This project provides personalized analysis and actionable recommendations to improve quiz performance. By analyzing historical, current, and recent quiz data, it identifies weak areas, highlights trends, and creates visualizations to guide students' preparation.

## Features
- **Performance by Topic**: Analyze scores, accuracy, and mistakes for each topic.
- **Current Quiz Analysis**: Detailed evaluation of the latest quiz submission.
- **Personalized Recommendations**: Suggest areas to focus on and maintain.
- **Insights**: Highlight weak areas, strong topics, and improvement trends.
- **Visualizations**:
  - Weak topics by accuracy.
  - Improvement trends over time.
  - Performance gaps by incorrect answer ratios.

## Setup Instructions

### Prerequisites
Ensure the following are installed:
- Python 3.7+
- Libraries:
  - pandas
  - json
  - matplotlib
  - seaborn

### Installation

   ```
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Place the following JSON files in the project directory:
   - `historical_quiz_data.json` (Historical quiz data for the user)
   - `quiz_submission_data.json` (Latest quiz submission data for the user)
   - `data.json` (Current quiz details)

### Usage
1. Run the script:
   ```bash
   python personalized_recommendations.py
   ```
2. Outputs:
   - **Insights and Recommendations**:
     - Saved to `quiz_insights_and_recommendations.csv`.
   - **Visualizations**:
     - `weak_topics_visualization.png`
     - `improvement_trends.png`
     - `performance_gaps.png`

## Approach Description

### Data Processing
1. **Load and Normalize**:
   - Load data from historical, current, and latest quizzes.
   - Flatten nested JSON structures to extract relevant information.
2. **Combine Data**:
   - Merge historical and latest quiz datasets for unified analysis.

### Analysis
1. **Performance Metrics**:
   - Calculate average scores, accuracy, and mistake counts by topic.
   - Identify weak and strong topics.
2. **Trends**:
   - Track accuracy trends over time.
   - Compare current quiz performance with historical data.
3. **Insights**:
   - Highlight weak areas with low accuracy or high mistakes.
   - Recognize strong topics with high accuracy and consistency.

### Recommendations
- Practice weak topics with targeted suggestions.
- Maintain performance in strong topics.
- Optimize preparation by focusing on specific difficulty levels or question types.

### Visualizations
1. **Weak Areas**:
   - Bar plot of topics with low accuracy.
2. **Improvement Trends**:
   - Line plot showing accuracy changes over time.
3. **Performance Gaps**:
   - Bar plot of incorrect answer ratios by topic.


## Contributing
Feel free to submit issues or pull requests to enhance the project.

## Contact
For questions or feedback, please contact Nishant sharma at nishant.jpis@gmail.com.
![image1](https://github.com/user-attachments/assets/8f488d70-a622-435f-ab27-b522368a3ed8)
