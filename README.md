# Threat Detection in Roman Urdu from YouTube and Reddit Comments

This project is designed to scrape comments from YouTube and Reddit using their respective APIs and detect potentially threatening content written in Roman Urdu. The entire pipeline is built in Python and runs in Google Colab for easy cloud execution.

## 📌 Features

- Scrapes comments using YouTube Data API and Reddit API (PRAW)
- Preprocesses comments: removes emojis, special characters, and HTML
- Detects threats using a comprehensive list of Roman Urdu keywords
- Labels comments as `threat` or `non-threat`
- Outputs structured `.csv` files for both platforms

---

## 🛠️ Tools & Libraries Used

- **Google Colab** – for development and execution
- **Python** – programming language
- **YouTube Data API v3** – to access YouTube comments
- **Reddit API (PRAW)** – to fetch Reddit comments
- **Pandas** – for data handling
- **Regular Expressions (re)** – for text cleaning
- **Emoji** – to remove emoji content

---

## 📂 Data Columns in CSV Output

| Platform | Post_ID | Content | Label |
|----------|---------|---------|-------|
| YouTube/Reddit | Video/Post ID | Cleaned Comment | threat / non-threat |

---

## 🔍 Roman Urdu Threat Keywords

A curated list of over 100 Roman Urdu keywords such as:

"mar dunga", "khatra", "maut", "beghairat", "kharab", "gandi", "qatal", "zinda nahi bachoge", "khatarnaak", "bandook", ...

These are used to flag comments containing potentially harmful language.

---

## 🚀 How to Run

1. Clone the repository.
2. Open the YouTube and Reddit scripts in Google Colab.
3. Enter your API keys:
   - YouTube API Key from Google Cloud Console.
   - Reddit credentials (Client ID, Secret, User Agent).
4. Execute the code cells sequentially.
5. Download the resulting CSV files.

---

## ⚠️ Limitations

- Facebook, Instagram, and Twitter data scraping was skipped due to API restrictions and account access issues.
- This is a keyword-based detection system and does not use machine learning or NLP models.

---

## 📁 Output

- `YouTube_Comments_Scrape.csv`
- `Reddit_Comment_Scrape.csv`

Each contains labeled comment data, ready for analysis or further processing.

 

## 📧 Author

**Hamza Afzal**  

Degree: BS(CS)  

University: Bahria University Islamabad
 
