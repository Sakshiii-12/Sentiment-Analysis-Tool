## Sentiment-Analysis-Tool

This project is designed to analyze and visualize the sentiment and emotional tone of textual data using Natural Language Processing (NLP) techniques.By combining rule-based analysis and machine learning-based scoring, this tool delivers both quantitative and qualitative insights, making it useful for academic research, mental health journaling, brand sentiment tracking, or content evaluation.


### Overview:
This project uses **Natural Language Processing (NLP)** to analyze sentiments and extract emotions from raw text. It features:
* **VADER (NLTK)** for rule-based sentiment analysis
* **TextBlob** for AI-based polarity scoring
* **Custom emotion detection** using a word-emotion dictionary
* **Dynamic visualizations**: bar charts, pie charts, word clouds
* **Adaptive color theming** based on detected sentiment


### How It Works:

1. **Text Preprocessing**
   * Convert to lowercase
   * Remove punctuation

2. **Tokenization & Stopword Removal**
   * Extract keywords

3. **Emotion Detection**
   * Match words from `emotions.txt`

4. **Sentiment Analysis**
   * **VADER** (rule-based)
   * **TextBlob** (AI-based polarity)

5. **Visualizations**
   * **Bar Chart** of emotion frequency
   * **Pie Chart** of emotion distribution
   * **Word Cloud** from emotion words

6. **Dynamic Color Scheme**
   * Green for positive
   * Red for negative
   * Orange/Yellow for neutral


### How to Run:

#### 1️. Setup
Install required libraries:

```bash
pip install textblob nltk wordcloud matplotlib
```

Download required NLTK data:

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('vader_lexicon')
```

#### 2️. Execute

* Open `Sentiment_Analysis.ipynb` in **Google Colab** ✅ *(Highly Recommended — works best without any local setup)*
  *(or run `sentiment_analysis.py` locally if preferred)*

#### 3️. Provide Input

* Place your `.txt` file (e.g., `GenZ.txt`) in the same directory
* Edit `emotions.txt` to customize emotion mappings
* Ensure the text files are in **UTF-8 encoding** for proper processing


### Project Structure:

```
sentiment-analysis
 ├── Sentiment_Analysis.ipynb    # Main notebook
 ├── sentiment_analysis.py       # Script version
 ├── GenZ.txt                    # Input text file
 ├── emotions.txt                # Word-emotion dictionary
 ├── results/                    # Auto-generated visualizations
 ├── README.md                   # Documentation
```


### Sample Output:
Sentiment Result: **Positive / Neutral / Negative**

TextBlob Score: e.g., **Polarity = 0.52**

- Emotion Bar Chart
- Emotion Word Cloud
- Emotion Pie Chart


### Color Scheme Explained:

| Sentiment | Primary Color | Theme        |
| --------- | ------------- | ------------ |
| Positive  | 🟢 Dark Green | Pastel Green |
| Negative  | 🔴 Dark Red   | Pastel Red   |
| Neutral   | 🟠 Orange     | Muted Orange |

Visual themes adapt based on the final sentiment to enhance clarity.


### Features:
- Text preprocessing & tokenization
- Dual sentiment analysis (VADER + TextBlob)
- Customizable emotion dictionary
- Sentiment-based dynamic color theming
- Informative visualizations
- Modular and clean code structure
- Best performance in **Google Colab** (no configuration required)


### Future Enhancements:

- Add **BERT/Transformer-based models** for deep sentiment detection
- Build a **Streamlit web app** for live sentiment/emotion input
- Connect with **Twitter, Reddit** for real-time scraping
- Plug into **chatbots or mental health tools** for mood tracking

### Applications:

- Customer feedback analysis
- Product or movie review sentiment monitoring
- Emotion recognition in therapy journals
- Sentiment tracking in news or tweets
- Emotion-aware chatbot conversations

### Output:

![Image](https://github.com/user-attachments/assets/d14b3c04-7835-447b-ad8b-981143d86e8e)


### Team Members

- Sakshi Makwana
- Jayal Shah
- Raj Patel
- Maynak Jangid
