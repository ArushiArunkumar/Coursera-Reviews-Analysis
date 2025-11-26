# Coursera Reviews Analysis
### *A Large-Scale Data Science & NLP Study of 1.4 Million Online Course Reviews*

**Project Website**: [To be updated]

---

# Overview

This project presents an analysis of 1.4 million Coursera course reviews, combining Data Science, Natural Language Processing (NLP), and data visualization techniques to recognise patterns in learner satisfaction, teaching quality, and course design effectiveness.

The project checks for: 
* quantitative trends - ratings, popularity, institutional performance) and 
* qualitative signals - sentiment, topics, review themes
They revealing deep insights into the dynamics of large-scale online education.

This work is intended to demonstrate high-level analytical capability suitable for research assistant positions, postgraduate coursework, and academic evaluation.

---

# Objectives

1. Clean & preprocess large-scale review data
2. Conduct exploratory analysis & identify global patterns
3. Evaluate how course popularity influences satisfaction
4. Extract positive and negative review themes using NLP
5. Perform topic modeling to identify teaching & structural patterns
6. Investigate institutional quality vs learner ratings
7. Build a polished website to present insights interactively

---

# Dataset Description

Two datasets were used:

* Coursera_courses.csv

  * course_id
  * name
  * institution
  * course_url

* Coursera_reviews.csv

  * course_id
  * reviews (text)
  * rating (1–5)
  * reviewer
  * date_reviews

After merging, the final dataset contained:

* 1,446,604 reviews
* 6,000+ courses
* 100+ institutions
* 10 years of timestamps

---

# Tech Stack

### Programming & Analysis

* Python (Pandas, NumPy)
* Matplotlib, Seaborn
* NLP: NLTK, VADER, Scikit-learn
* Topic Modeling: LDA

---

# Major Components

## 1. Data Cleaning & Preparation

* Removal of duplicates & corrupted entries
* Standardization of text fields
* Stopword removal, tokenization, lemmatization
* Sentiment score generation (VADER)
* Extraction of temporal features (year-month)
* Creation of course-level aggregates:

  * average rating
  * rating variance
  * review count (popularity metric)

---

## 2. Exploratory Data Analysis

Key visualizations included:

* Rating distribution
* Review count distribution
* Popularity vs average rating
* Popularity vs rating variance
* Monthly rating trends
* Institution-level comparisons

All visualizations are available under **EDA** on the project website.

---

## 3. NLP Analysis

### Sentiment Modeling

Sentiment polarity correlates strongly with course ratings, providing a more granular perspective than numerical ratings alone.

### Word Clouds

Distinct themes emerge between 5-star and 1-star reviews:

* Positive: clarity, usefulness, instructor quality
* Negative: assignments, outdated content, confusing lectures

### Topic Modeling (LDA)

Five core thematic clusters appear:

1. Real-world applications
2. Assignment & structural issues
3. Beginner-friendly programming
4. Instructor praise & enjoyment
5. Spanish-language positive reviews

Detailed topic summaries appear on the **NLP** page.

---

## 4. Insights

This project focuses on four high-impact research insights:

---

### Popularity Reduces Satisfaction (Polarization Effect)

* Correlation between popularity (review_count) and average rating ≈ **–0.10**
* Correlation between popularity and rating variance ≈ **+0.09**
* Highly popular courses attract more diverse learner backgrounds →
  **higher disagreement and slightly lower satisfaction**
* Niche courses with small, homogeneous audiences consistently score higher

This supports the educational psychology principle of **audience dilution**.

---

### Positive vs Negative Review Themes (Teaching Quality Matters Most)

**Positive reviews** highlight:

* Clear explanations
* Helpful instructors
* Well-structured content
* Strong learning outcomes

**Negative reviews** focus on:

* Assignment difficulty & unclear instructions
* Outdated material
* Fast/unclear teaching
* Poor lecture quality

**Conclusion:**
Learners react primarily to **pedagogical clarity**, not the subject matter itself.

---

### Difficulty Strongly Influences Ratings

Advanced courses produce more negative sentiment due to:

* Fast pacing
* Dense theoretical material
* Insufficient examples

Beginner-friendly courses consistently rank highest.

This reflects the **Inverted-U Learning Curve**:

> Too easy → boring
> Just right → satisfying
> Too hard → overwhelming → negative ratings

---

### Institutional Prestige ≠ Course Quality

* Top-rated courses come from a mix of elite universities, mid-tier institutions, and industry leaders
* Global ranking does **not** predict course quality
* Instructor clarity and course design are far more important

MOOCs **democratize quality** — good teaching outweighs university branding.

---


# Conclusion

This project demonstrates how large-scale learner feedback can uncover:

* structural deficiencies in online courses
* strengths in teaching practices
* patterns in learner psychology
* dynamics between popularity and satisfaction
* the democratization of educational quality online

The findings have strong implications for:

* Course designers
* Curriculum researchers
* Instructors
* MOOC platforms

---

# Future Work

Planned extensions include:

* BERTopic / modern topic modeling
* Instructor-level sentiment profiling
* Course quality scoring model
* Interactive review explorer
* Summarization of reviews using transformers
* Predicting ratings from review text
* Causal modeling of learning outcomes

---

# Acknowledgments

Data sourced from Coursera course review datasets on [Kaggle](https://www.kaggle.com/datasets/imuhammad/course-reviews-on-coursera?resource=download).
Analysis, visualizations, and website authored by Arushi Arunkumar.

---

# Contact

For collaborations or feedback:\
[arushiarunkumar@gmail.com](mailto:arushiarunkumar@gmail.com)\
[LinkedIn](https://www.linkedin.com/in/arushi-arunkumar/)\
[GitHub](https://github.com/ArushiArunkumar)

