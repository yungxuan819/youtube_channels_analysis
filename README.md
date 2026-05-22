# 📺 YouTube Channels Analysis & Prediction

A data analysis and machine learning project that explores key performance statistics from the **top 5,000 YouTube channels** — uncovering what drives channel success through EDA and visualizations, and building regression models to predict the **average views** per video of a channel.

---

## 📁 Project Structure

```
youtube_channels_analysis/
│
├── youtube-channels-analysis.ipynb    # Main notebook: data cleaning, EDA & prediction models
└── top-5000-youtube-channels.csv      # Dataset: top 5,000 YouTube channels by subscriber count
```

---

## 📊 Dataset

The dataset contains statistics for the **top 5,000 YouTube channels**, sourced from the [Top 5000 YouTube Channels Dataset on Kaggle](https://www.kaggle.com/datasets/surajjha101/top-youtube-channels-data).

| Column | Description |
|--------|-------------|
| `rank` | Channel rank by subscriber count |
| `channel_name` | Name of the YouTube channel |
| `category` | Content category (e.g. Music, Gaming, Entertainment) |
| `subscribers` | Total number of subscribers |
| `views` | Total lifetime views on the channel |
| `total_videos` | Total number of videos uploaded |
| `average_views` | Average views per video — **target variable** |
| `country` | Country of origin of the channel |

---

## 🔍 Project Overview

### Data Cleaning
- Handling missing values in category and country columns
- Parsing and converting numeric fields stored as strings (e.g. "1.2M", "500K")
- Removing or imputing outliers in views and subscriber counts

### Exploratory Data Analysis (EDA)
- Distribution of subscribers and views across the top 5,000 channels
- Top-performing categories by average views and subscriber count
- Country-level breakdown of channel representation
- Correlation between total videos, subscribers, views, and average views
- Identifying what separates high-average-view channels from low ones

### Prediction Models
- Regression models trained to predict `average_views` per video
- Feature engineering and selection based on EDA findings
- Model comparison and evaluation using R², MAE, and RMSE

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook

### Installation

```bash
git clone https://github.com/yungxuan819/youtube_channels_analysis.git
cd youtube_channels_analysis
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Run

```bash
jupyter notebook youtube-channels-analysis.ipynb
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| pandas | Data loading & manipulation |
| NumPy | Numerical operations |
| matplotlib / seaborn | Data visualizations |
| scikit-learn | Regression models & evaluation |
| Jupyter Notebook | Development environment |
