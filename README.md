# Wordle Data Analytics Project

A comprehensive data analysis of Wordle game patterns using Twitter data, featuring visualization of player strategies, guess patterns, and performance metrics.

## 📊 Project Overview

This project analyzes Wordle gameplay data from Twitter to uncover interesting patterns and insights about how people play the popular word game. The analysis includes:

- **Tweet Volume Analysis**: Daily Wordle tweet patterns over time
- **Attempt Distribution**: How many tries it takes players to solve puzzles
- **Guess Pattern Analysis**: Detailed breakdown of correct, misplaced, and incorrect letters by attempt
- **Letter Frequency Analysis**: Most common correct letters in first guesses
- **Performance Visualization**: Interactive charts and styled tables

## ⚠️ Dataset Access

This project uses the "Wordle Tweets" dataset by Ben Hamner from Kaggle.
Due to licensing restrictions, the dataset is not included here.
You can access it by creating a Kaggle account and downloading it directly:
https://www.kaggle.com/datasets/benhamner/wordle-tweets

## 🛠️ Requirements

### Python Dependencies

```
pandas
numpy
matplotlib
seaborn
jinja2
```

### Installation

Install the required packages using pip:

```bash
pip install pandas numpy matplotlib seaborn jinja2
```

## 📁 Project Structure

```
Wordle/
├── Wordle DS project.ipynb    # Main Jupyter notebook with analysis
├── tweets.csv                 # Wordle tweets dataset (download separately)
└── README.md                  # This file
```

## 🚀 Getting Started

1. **Download the Dataset**:

   - Go to [Kaggle Wordle Tweets Dataset](https://www.kaggle.com/datasets/benhamner/wordle-tweets)
   - Download `tweets.csv` and place it in the project directory

2. **Install Dependencies**:

   ```bash
   pip install pandas numpy matplotlib seaborn jinja2
   ```

3. **Run the Notebook**:
   - Open `Wordle DS project.ipynb` in Jupyter Notebook or VS Code
   - Execute cells sequentially from top to bottom

## 📈 Analysis Features

### 1. Data Processing

- Parses Wordle tweet text to extract game information
- Standardizes emoji representations (⬜ → ⬛)
- Extracts attempt numbers, dates, and guess patterns

### 2. Visualizations

#### Tweet Volume Over Time

- Line chart showing daily Wordle tweet activity
- Helps identify trends and peak engagement periods

#### Attempt Distribution

- Horizontal bar chart of solve attempts (1-6 tries)
- Shows the distribution of player performance

#### Guess Pattern Analysis

- Styled heatmap showing attempts vs. success rate
- Three-panel visualization comparing correct, misplaced, and incorrect letters
- Average performance metrics by guess number

#### Letter Analysis

- Bar chart of most common correct letters in first guesses
- Insights into popular starting word strategies

### 3. Interactive Elements

- Gradient-styled tables using pandas styling
- Color-coded visualizations with consistent theming
- Professional chart formatting with proper labels and titles

## 🔍 Key Insights

The analysis reveals:

- **Popular Starting Strategies**: Which letters appear most often in successful first guesses
- **Performance Patterns**: How success rates change with each attempt
- **Temporal Trends**: Daily engagement patterns over time
- **Guess Efficiency**: Average number of correct/misplaced/incorrect letters per attempt

## 🎨 Visualization Style

The project uses:

- **ggplot style** for consistent, professional-looking charts
- **Color palette cycling** for multi-panel visualizations
- **Gradient backgrounds** for data tables
- **Proper spacing and labels** for clarity

## 📊 Data Structure

The processed dataset includes:

- `wordle_id`: Puzzle number
- `tweet_date`: Date of the tweet
- `n_attempts`: Number of attempts to solve
- `guess1-6`: Individual guess patterns
- `guess1-6_correct/wrong_spot/incorrect`: Letter counts by category
- `answer`: The correct word for each puzzle (subset)

## 🤝 Contributing

Feel free to fork this project and submit pull requests for:

- Additional analysis features
- Improved visualizations
- Code optimizations
- Documentation improvements

## 📝 License

This project is for educational and research purposes. Please respect the original dataset's licensing terms from Kaggle.

## 🙏 Acknowledgments

- **Ben Hamner** for providing the Wordle Tweets dataset on Kaggle
- **Wordle** game by Josh Wardle for inspiring this analysis
- **Twitter users** who shared their Wordle results, making this analysis possible

---

_Happy analyzing! 🎯_
