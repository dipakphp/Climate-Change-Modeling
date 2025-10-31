# 🌍 Climate Change Modeling

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

This project performs **sentiment and discourse analysis** on public comments from NASA’s official Facebook page about climate change. The goal is to understand public perception, engagement trends, and dominant discussion themes using **Natural Language Processing (NLP)** and **Machine Learning** techniques.

> 🔍 **Note**: Despite the title "Climate Change Modeling", this project focuses on **social sentiment modeling**, not physical climate system prediction. It aligns with Part A of the provided project brief (sentiment analysis on social media data).

---

## 📁 Dataset

- **Source**: [NASA Climate Change Facebook Page](https://web.facebook.com/NASAClimateChange/)
- **Time Range**: 2020 – 2023
- **Size**: 500+ anonymized user comments
- **Columns**:
  - `date`: Timestamp of comment
  - `text`: Comment content
  - `likesCount`: Number of likes
  - `commentsCount`: Number of replies
  - `ProfileName`: SHA-256 hashed (privacy-preserving)

> 🔒 All user identities are anonymized per ethical data practices.

---

## 🧠 Key Analyses Performed

1. **Sentiment Analysis**
   - Dual-model approach: **TextBlob** + **VADER**
   - Categorized as *Positive*, *Neutral*, or *Negative*
2. **Temporal Trend Analysis**
   - Sentiment shifts over months/years
3. **Engagement Insights**
   - Correlation between likes, replies, and sentiment
   - Most active days/years
4. **Topic Modeling**
   - **LDA (Latent Dirichlet Allocation)** to uncover 5 key discussion themes
5. **N-gram & Keyword Extraction**
   - Top bigrams/trigrams in public discourse
6. **Machine Learning Classification**
   - **Random Forest** model to classify sentiment from text (TF-IDF features)
   - Evaluation via classification report & confusion matrix
7. **Visualizations**
   - Word clouds by sentiment
   - Time-series plots
   - Bar charts, histograms, heatmaps

---

## 🛠️ Technologies & Libraries

- **Core**: Python, Pandas, NumPy
- **NLP**: NLTK, TextBlob, VADER, scikit-learn (TF-IDF, CountVectorizer)
- **ML**: Random Forest Classifier, LabelEncoder
- **Topic Modeling**: LDA, NMF
- **Visualization**: Matplotlib, Seaborn, WordCloud
- **Environment**: Jupyter Notebook / Google Colab

---

## 📦 Installation & Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/dipakphp/climate-change-sentiment.git
   cd climate-change-sentiment
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset:
   - Get `climate_nasa.csv` from the [project PDF link](#) (or your local copy)
   - Place it in the root directory

4. Run the notebook:
   ```bash
   jupyter notebook Climate_Change.ipynb
   ```

---

## 📄 Output

- Final enriched dataset: `climate_comments_analyzed.csv`
  - Includes cleaned text, sentiment scores, categories, dominant topics, and engagement metrics
- Comprehensive visual reports on public sentiment and discourse patterns

---

## 📝 Ethical Note

This project treats climate change discourse with neutrality and respect for diverse viewpoints, as emphasized in the original dataset documentation. No attempt is made to influence or judge opinions—only to analyze and understand them.

---

## 📚 References

- NASA Climate Change Communications: [https://climate.nasa.gov/](https://climate.nasa.gov/)
- VADER Sentiment: Hutto, C.J. & Gilbert, E.E. (2014)
- TextBlob: https://textblob.readthedocs.io/
- LDA Topic Modeling: Blei, D.M., Ng, A.Y., & Jordan, M.I. (2003)

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

## 🙌 Acknowledgements

- Thanks to **NASA** for fostering open public dialogue on climate change.
- Dataset curators for ethical anonymization and accessibility.

---

> ✨ **Project completed as part of an Advanced Data Science initiative**  
> 🌱 Understanding public sentiment is a critical step toward effective climate communication.
