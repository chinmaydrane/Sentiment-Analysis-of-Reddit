# Reddit Sentiment & Tone Analysis

## 📌 Overview
This project analyzes the sentiment and tone of Reddit comments related to a specific subject using *Python, NLP, and AsyncPRAW. The analysis is performed using **TextBlob* and *VADER*, providing insights into sentiment polarity (Positive, Negative, Neutral) and tone classification (Formal vs Informal).

## 🚀 Features
- *Scrapes Reddit comments* using *AsyncPRAW* based on a given subject name and code.
- *Performs sentiment analysis* using:
  - *TextBlob* (Polarity & Subjectivity Analysis)
  - *VADER* (Lexicon-Based Sentiment Scoring)
- *Classifies comments as Formal or Informal* using keyword-based heuristics.
- *Generates Pie Charts* for visualization.
- *Exports results to an Excel file* with embedded charts.

## 🛠 Technologies Used
- *Python* - Programming Language
- *AsyncPRAW* - Reddit API Wrapper
- *TextBlob* - NLP Sentiment Analysis
- *VADER (NLTK)* - Sentiment Scoring
- *Matplotlib* - Data Visualization
- *Pandas* - Data Handling
- *OpenPyXL* - Excel File Manipulation

## 📌 Installation & Setup
### 🔹 Prerequisites
Ensure you have *Python 3.x* installed along with the required dependencies.

### 🔹 Install Dependencies
sh
pip install asyncpraw pandas matplotlib textblob nltk openpyxl


### 🔹 Download NLTK Lexicon
python
import nltk
nltk.download('vader_lexicon')


## 📌 Usage
Run the script and enter the subject details when prompted:
sh
python reddit_sentiment_analysis.py

### 🎯 Example Input

Enter the subject name: Machine Learning
Enter the subject code: ML101


### 📊 Output
- *Excel File:* async_sentiment_analysis_results.xlsx (Contains sentiment analysis results + embedded charts)
- *Pie Charts:*
  - *TextBlob Sentiment Analysis* (textblob_sentiment.png)
  - *VADER Sentiment Analysis* (vader_sentiment.png)
  - *Tone Analysis* (tone_analysis.png)

## 📌 How It Works
1. *Reddit Scraping*: Fetches comments from the r/india subreddit based on the subject query.
2. *Text Cleaning*: Removes unwanted characters (mentions, links, special symbols).
3. *Sentiment Analysis*:
   - *TextBlob: Determines **polarity* (positive, negative, neutral).
   - *VADER*: Computes sentiment scores using lexicon-based analysis.
4. *Tone Classification*:
   - Detects *informal* language using predefined keywords.
   - Assesses sentence complexity for *formal* tone classification.
5. *Data Visualization & Export*:
   - Generates *pie charts* for sentiment & tone distribution.
   - Saves results in an *Excel file* with embedded charts.

## 📌 License
This project is licensed under the *MIT License*. Feel free to use and modify it.


## 📌 Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue.

---
💡 *Star this repo* if you find it useful! ⭐
