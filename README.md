# 📺 YouTube Scraping Project

## 📌 Overview

This project focuses on **scraping, preprocessing, and analyzing YouTube video data** using Python. It extracts useful information such as video titles, views, and duration from a YouTube channel and transforms it into a structured format for further analysis and visualization.

The workflow includes:

* Web scraping from YouTube
* Data cleaning and preprocessing
* Text processing
* Data visualization

---

## 🚀 Features

* Scrapes latest videos from a YouTube channel
* Extracts:

  * Video Titles
  * View Counts
  * Video Duration
* Saves data into an Excel file
* Cleans and preprocesses raw data
* Performs text preprocessing on titles
* Generates insightful visualizations:

  * Word Cloud
  * Top viewed videos
  * Duration-based distribution

---

## 🛠️ Tech Stack

* **Python**
* **Libraries Used:**

  * `requests`
  * `beautifulsoup4`
  * `pandas`
  * `xlsxwriter`
  * `matplotlib`
  * `seaborn`
  * `nltk`
  * `wordcloud`

---

## 📂 Project Structure

```
YouTube-Scraping-Project/
│
├── youtube_scraper.py       # Web scraping script
├── preprocessing.py         # Data cleaning and preprocessing
├── visualization.py         # Data visualization scripts
├── youtube_videos.xlsx      # Scraped dataset
├── README.md                # Project documentation
```

---

## ⚙️ Installation

Install required libraries:

```bash
pip install requests beautifulsoup4 pandas xlsxwriter matplotlib seaborn nltk wordcloud
```

---

## 📥 How It Works

### 1. Web Scraping

* Sends an HTTP request to a YouTube channel page
* Extracts embedded JSON (`ytInitialData`)
* Parses video metadata:

  * Title
  * Views
  * Duration

### 2. Data Storage

* Stores extracted data into an Excel file (`youtube_videos.xlsx`)

### 3. Data Preprocessing

* Cleans `Views` column:

  * Converts text (e.g., "1.2K") → numeric
* Converts `Duration` into seconds
* Categorizes videos:

  * Mini-Videos (< 15 mins)
  * Long-Videos (< 1 hour)
  * Very-Long-Videos (> 1 hour)

### 4. Text Preprocessing

* Lowercasing text
* Removing URLs & special characters
* Tokenization
* Stopword removal
* Stemming

### 5. Data Visualization

* 📊 Word Cloud of titles
* 📈 Top 3 most viewed videos
* 📉 Video count by duration category

---

## 📊 Output Examples

* Word Cloud showing popular keywords
* Bar chart of top-performing videos
* Count plot of video duration categories

---

## ▶️ Usage

Run the scripts step by step:

```bash
python youtube_scraper.py
python preprocessing.py
python visualization.py
```

---

## ⚠️ Disclaimer

* This project is for **educational purposes only**
* YouTube structure may change, which can break the scraper
* Always follow YouTube’s **Terms of Service**

---

## 💡 Future Improvements

* Use YouTube Data API for reliability
* Add sentiment analysis on titles/comments
* Build dashboard using Streamlit or Power BI
* Automate periodic data collection

---

## 🤝 Contribution

Contributions are welcome! Feel free to fork the repo and submit a pull request.

---

## 📬 Contact

For any queries or suggestions, feel free to reach out.

---

⭐ *If you found this project useful, consider giving it a star!*
