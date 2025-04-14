# Financial-News-Sentiment-Analysis

#News Sentiment Analyzer
A Python tool that analyzes sentiment in news articles about any topic using FinBERT, providing visualizations and comprehensive reports.

# Overview
This tool collects news articles about any specified topic using NewsAPI and analyzes their sentiment using the FinBERT model. It extracts full text from articles, summarizes each one, and classifies them as positive, neutral, or negative. The tool then generates comprehensive visualizations, an interactive HTML report, and CSV data showing sentiment trends across all collected articles.

# Features

Flexible Topic Analysis: Analyze news sentiment for any topic of your choice
Advanced Sentiment Analysis: Uses FinBERT, a financial domain-specific BERT model
Comprehensive Visualizations:

- Sentiment distribution pie chart
- Sentiment count bar chart
- Timeline of articles by publication date and sentiment
- Score distribution boxplots
- Article-by-article stacked sentiment charts


Multiple Report Formats:

- Interactive HTML report with all visualizations and detailed article summaries
- CSV export with complete sentiment data


# Installation

- Clone this repository:
bashgit clone https://github.com/yourusername/news-sentiment-analyzer.git
cd news-sentiment-analyzer

- Install the required packages:
bashpip install requests pandas numpy matplotlib transformers torch newspaper3k nltk tqdm

- Obtain a NewsAPI key:

Sign up for a free API key at NewsAPI
You'll need this key to fetch news articles




# How It Works

Data Collection: Fetches articles from NewsAPI based on your search query
Text Extraction: Uses newspaper3k to extract full text from each article URL
Sentiment Analysis: Applies FinBERT to analyze sentiment in each article
Summarization: Creates extractive summaries of each article
Visualization: Generates multiple visualizations of the sentiment data
Reporting: Creates comprehensive reports in multiple formats

# Limitations 

- NewsAPI Restrictions: The free tier of NewsAPI only provides access to articles from the past 30 days and has a limited number of requests per day.
- Simple Summarization: The current extractive summarization method simply takes the first few sentences of an article, which may not capture the most important information.
- Language Limitation: Currently only analyzes English language articles.
- No Paywalled Content: Cannot access articles behind paywalls or those requiring login credentials.
- Static Analysis: The tool performs a one-time analysis rather than continuous monitoring over time.

# Future Work
- Web Application Development: Create a full-fledged web application with a user interface for more interactive analysis.
- Multiple News API Support: Integrate alternative news sources like GDELT, MediaStack, or directly scraping news sites to overcome the 30-day limitation.
- Enhanced Sentiment Analysis: Implement domain-specific sentiment models for different topics
- Advanced NLP Features
- Social Media Integration: Incorporate sentiment from Twitter, Reddit, and other social platforms





# Acknowledgments

NewsAPI for providing the news article data
FinBERT for the sentiment analysis model
newspaper3k for article extraction
Hugging Face for the transformers library

# Contact
If you have any questions or suggestions, please open an issue or reach out to abdulwasii.ajayi@gmail.com

