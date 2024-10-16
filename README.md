# Predicting Premier League Match Outcomes Using Machine Learning

This project leverages machine learning to predict the outcomes of Premier League matches using an XGBoost model. The goal is to provide probabilities for Home Wins, Away Wins, and Draws based on past match statistics.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model](#model)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/Predicting-Premier-League-Match-Outcomes-Using-Machine-Learning.git
    ```

2. Navigate to the project directory:
    ```bash
    cd Predicting-Premier-League-Match-Outcomes-Using-Machine-Learning
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Prepare your dataset (`seasonstats.csv` and `matches.csv`).
2. Run the model training script:
    ```bash
    python predict_matches.py
    ```
3. Use the `predict_match_result(home_team, away_team)` function in the code to predict a match result:
    ```python
    predict_match_result('Manchester United', 'Liverpool')
    ```

The prediction will output probabilities for the match outcome and display a bar chart showing the chances of Home Win, Away Win, or Draw.

## Dataset

- `seasonstats.csv`: Contains season-specific statistics.
- `matches.csv`: Contains individual match details including goals, teams, etc.

## Model

We use an **XGBoost Classifier** to predict the outcome of a match (Win, Lose, or Draw). The model uses features such as:

- xG (expected goals)
- Attendance
- GF (goals for)
- GA (goals against)

## Features

- Predict match outcomes (Win, Lose, Draw) between two teams.
- Display probabilities as a bar chart for better visualization.
  
## Contributing

Feel free to contribute to this project by opening a pull request. You can also report issues or suggest new features.

## License

This project is licensed under the MIT License.
