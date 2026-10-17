# Airline Tweet Sentiment Analysis Dashboard

An interactive dashboard built with **Python** and **Streamlit** to explore sentiment in tweets about US airlines. It helps users examine overall sentiment, compare airlines, inspect tweet activity by hour, and explore common words in positive, neutral, and negative tweets.

## Features

- **Sentiment overview:** View the number of positive, neutral, and negative tweets as a bar chart or pie chart.
- **Airline comparison:** Compare tweet volumes across airlines.
- **Sentiment by airline:** Select airlines and compare the sentiment distribution.
- **Hourly exploration:** Filter tweets by the hour they were created and inspect available location data.
- **Random tweet:** Display a sample tweet for a selected sentiment.
- **Word clouds:** Explore common words in tweets for a selected sentiment.

## Built With

- Python
- Streamlit
- Pandas
- NumPy
- Plotly
- Matplotlib
- WordCloud

## Project Files

```text
streamlit-sentiment-dashboard/
├── app.py
├── requirements.txt
├── Tweets.csv
└── README.md
```

## Getting Started

### 1. Clone the repository

Replace `YOUR-USERNAME` with your GitHub username:

```bash
git clone https://github.com/YOUR-USERNAME/streamlit-sentiment-dashboard.git
cd streamlit-sentiment-dashboard
```

### 2. Create and activate a virtual environment (recommended)

**macOS / Linux**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Check the dataset path

Keep `Tweets.csv` in the project directory alongside `app.py`. In `app.py`, the data path should be relative:

```python
DATA_URL = "Tweets.csv"
```

The app expects the CSV to contain columns used by the dashboard, including `tweet_created`, `airline_sentiment`, `text`, `airline`, and any location fields used by the map view.

### 5. Run the dashboard

```bash
streamlit run app.py
```

Streamlit will show a local URL in the terminal. Open it in your browser to use the dashboard.

## Deploying

You can deploy the app using [Streamlit Community Cloud](https://share.streamlit.io/):

1. Push `app.py`, `requirements.txt`, `Tweets.csv` (if its size and usage rights permit), and this `README.md` to your GitHub repository.
2. Sign in to Streamlit Community Cloud with GitHub.
3. Create a new app and select this repository and the `main` branch.
4. Set the main file path to `app.py`, then deploy.

## Notes

- The dashboard analyzes the dataset provided with this project; results depend on the contents and quality of that data.
- Ensure the dataset's license and usage terms allow you to publish it publicly before committing it to a public repository.
- Avoid committing secrets, access tokens, or private data.
- If you add or change Python packages, update `requirements.txt` accordingly.

## Future Improvements

- Add keyword search and date filters.
- Add sentiment percentage summaries and additional visual comparisons.
- Improve layout and accessibility for mobile screens.
- Add automated data validation and clearer error messages.

## Author

Created as a Python data analytics project. Feel free to adapt this section with your name, portfolio, or LinkedIn profile.
