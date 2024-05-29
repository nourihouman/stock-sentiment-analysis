# stock-sentiment-analysis
This project analyzes sentiment in financial news headlines from Reuters, CNBC, and The Guardian from the year 2018. The goal is to determine whether there's a correlation between daily news sentiment and S&P 500 stock market movements.

## Data Sources (https://www.kaggle.com/datasets/notlucasp/financial-news-headlines/discussion/236127)
- **Reuters Headlines**
- **CNBC Headlines**
- **The Guardian Headlines**

## Methodology
1. **Data Loading**: Load historical news headlines from Reuters, CNBC, and The Guardian.
2. **Data Preprocessing**:
   - Convert all text to lowercase.
   - Remove punctuation and special characters.
   - Clean dara
3. **Sentiment Analysis**:
   - Initially, VADER sentiment analysis tool was employed to calculate sentiment scores for news headlines.
   - Sentiment data was then merged with S&P 500 closing prices to analyze correlations.
4. **BERT Model**:
   - Setup a BERT model to perform a more nuanced sentiment analysis.
   - Again, merge these sentiment results with S&P 500 data for correlation analysis.
  
## Results
Both VADER and BERT sentiment analysis models show a weak correlation with S&P 500 price movements, suggesting that daily sentiment in news headlines may not have a strong predictive power on stock prices over the observed period.

## Discussion and Future Work
- **Non-linear Relationships**: The correlation analysis does not account for non-linear relationships. Future analysis might include more complex statistical methods or machine learning models.
- **Use of Descriptions**: News descriptions may provide richer information compared to headlines. Repeating the analysis using full article descriptions could yield different insights.
- **Shorter Time Frames**: Analyzing sentiment and stock prices over shorter intervals (e.g., weekly) might reveal more granular patterns not apparent in daily or annual data.

## How to Use This Repository
Clone the repository, install the required Python packages listed in `requirements.txt`, and run the Jupyter notebooks provided to see the analysis steps and reproduce the results.

