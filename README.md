# Fan Momentum Index (FMI)

A multimodal football analytics system that quantifies crowd momentum using real-time social media sentiment, tweet volume, and stadium audio intensity.

---

# Project Overview

Football fan energy is widely believed to influence match momentum, player psychology, and even refereeing decisions. However, quantifying collective crowd momentum in real time remains a major challenge in sports analytics.

This project introduces the **Fan Momentum Index (FMI)** — a data-driven framework that combines:

- Twitter sentiment analysis
- Tweet engagement volume
- Stadium crowd audio intensity

to generate a real-time momentum score during football matches.

The system was designed as an applied sports analytics and big data project focused on understanding and visualizing collective fan behavior during high-stakes football events.

---

# Core Concept

The Fan Momentum Index (FMI) integrates multiple real-time data streams into a unified metric representing crowd energy and engagement.

The index combines:

- Sentiment polarity from live tweets
- Tweet activity volume
- Stadium crowd noise intensity

to generate a normalized momentum score between 0 and 1.

---

# Objectives

The project aims to:

- Quantify fan engagement during football matches
- Analyze real-time crowd sentiment shifts
- Detect momentum spikes during key match events
- Correlate social media activity with crowd noise
- Build a scalable multimodal sports analytics pipeline
- Visualize fan momentum over time

---

# Tech Stack

## Programming & Analytics
- Python
- Pandas
- NumPy

## Natural Language Processing (NLP)
- VADER Sentiment Analysis
- NLTK

## Visualization
- Matplotlib
- Seaborn

## Audio Analytics
- Audio intensity extraction
- Signal normalization
- Decibel trend analysis

## Development Environment
- Jupyter Notebook

---

# Repository Structure

```text
fan-momentum-index/
│
├── data/
│   ├── audio/
│   │   └── match_audio_volume_by_second.csv
│   │
│   ├── processed/
│   │   ├── final_fmi_dataset.csv
│   │   ├── tweet_sentiment_by_minute.csv
│   │   └── Final_Aligned_Tweet_Dataset.csv
│   │
│   └── raw/
│
├── notebooks/
│   ├── fmi_extract_tweets.ipynb
│   ├── sentiment_scoring.ipynb
│   ├── final_fmi_dataset.ipynb
│   └── Finalndex.ipynb
│
├── visualizations/
│
└── README.md
```

---

# Dataset Overview

The project uses multiple synchronized datasets generated from football match data streams.

## Included Datasets

### Final Aligned Tweet Dataset
Contains processed tweets aligned minute-by-minute with match events.

Key features:
- Tweet timestamps
- Engagement metrics
- Event alignment
- Match timeline mapping

---

### Tweet Sentiment by Minute
Aggregated sentiment scores calculated from live tweet streams.

Key features:
- Average sentiment per minute
- Sentiment polarity trends
- Emotional momentum tracking

---

### Match Audio Volume by Second
Crowd audio intensity extracted from football match broadcasts.

Key features:
- Second-by-second crowd volume
- Crowd reaction spikes
- Stadium energy trends

---

### Final FMI Dataset
Final integrated dataset combining:
- Tweet sentiment
- Tweet volume
- Crowd audio intensity
- Match event alignment

This dataset powers the final Fan Momentum Index calculation.

---

# Methodology

## 1. Tweet Extraction & Alignment

Tweets were collected and aligned with:
- Match timestamps
- Key football events
- Minute-level aggregation windows

The pipeline filters and structures football-related fan activity for analysis.

---

## 2. Sentiment Analysis

Sentiment analysis was performed using the VADER NLP framework.

Processing steps included:
- Text cleaning
- Tokenization
- Sentiment scoring
- Minute-level aggregation

The output generated:
- Positive sentiment trends
- Negative sentiment spikes
- Overall emotional momentum

---

## 3. Audio Analytics

Crowd audio intensity was analyzed using:
- Signal normalization
- Volume extraction
- Time-series alignment

The resulting crowd energy signals were synchronized with:
- Match events
- Twitter sentiment
- Engagement spikes

---

## 4. Fan Momentum Index Construction

The final FMI score combines:

- Sentiment Score
- Tweet Volume
- Crowd Audio Energy

into a normalized momentum metric.

### FMI Formula

```text
FMI_t = α · norm(Sentiment_t)
      + β · norm(TweetVolume_t)
      + γ · norm(Audio_t)
```

where:
- α, β, γ represent weighted importance values
- all variables are normalized between 0 and 1

---

# Key Features

- Real-time fan momentum tracking
- Multimodal data fusion
- Social sentiment analytics
- Crowd audio analysis
- Event-aligned visualization
- Football engagement intelligence

---

# Visualizations Included

The project includes visualizations for:

- Tweet sentiment evolution
- Crowd audio intensity trends
- Fan momentum fluctuations
- Match event overlays
- Momentum spike detection

---

# Key Insights

The analysis revealed:

- Major football events generate synchronized spikes in sentiment and crowd intensity.
- Tweet activity and stadium audio frequently correlate during high-emotion moments.
- Crowd momentum can be quantitatively modeled using multimodal data streams.
- Momentum drops and surges can be identified in near real time.

---

# Potential Applications

The FMI framework can support:

## Football Clubs
- Fan engagement analytics
- Match atmosphere analysis
- Stadium orchestration systems

## Broadcasters
- Live momentum overlays
- Audience engagement enhancements

## Sports Analytics
- Crowd psychology research
- Event-response modeling
- Real-time engagement scoring

---

# Future Improvements

Potential future enhancements include:

- Real-time streaming dashboards
- Advanced transformer-based NLP models
- Live API integration
- Multilingual sentiment analysis
- Crowd chant detection
- Predictive momentum forecasting
- Interactive dashboards using Plotly or Power BI

---

# Files Included

## Datasets
- Tweet sentiment datasets
- Audio intensity datasets
- Final integrated FMI dataset

## Notebooks
- Tweet extraction pipeline
- Sentiment scoring workflow
- FMI calculation notebooks

## Visualizations
- Momentum graphs
- Sentiment trends
- Audio intensity plots

---

# Note

This project was originally developed as part of a collaborative university research initiative focused on real-time football fan analytics. This repository primarily contains the analytical workflows, datasets, and implementation components developed and organized by the author.

---

# Key References

- Patel & Passi (2020) — Real-Time Twitter Sentiment in Football
- Gautam et al. (2022) — Audio Intensity Analysis in Sports
- Wang & Qin (2023) — Crowd Influence and Home Advantage

---

# Author

Faiz Nizamuddin Karol

LinkedIn: https://linkedin.com/in/faiz-karol
