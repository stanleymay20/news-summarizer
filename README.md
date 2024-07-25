# news-summarizer
The News Summarizer is an AI-powered application that collects news articles from multiple sources, summarizes them, and posts the summaries to a website automatically every day at 8:00 AM. It uses machine learning models for text summarization, making news consumption more efficient.

# News Summarizer

## Brief Description

The News Summarizer is an AI-powered application that collects news articles from various sources, summarizes them, and posts the summaries to a website automatically every day at 8:00 AM. This project leverages machine learning models for text summarization and aims to help users quickly grasp the main points of news articles without reading the entire text.

## Table of Contents

- [Problem Statement](#problem-statement)
- [High-Level System Design](#high-level-system-design)
- [Detailed Design, Implementation, and Analysis](#detailed-design-implementation-and-analysis)
- [Evaluation](#evaluation)
- [Final Discussion](#final-discussion)
- [How to Deploy](#how-to-deploy)
- [How to Use](#how-to-use)
- [License](#license)

## Problem Statement

### Overview

The underlying business problem is the need for efficient news consumption. In the fast-paced world, users often do not have the time to read through lengthy news articles. Summarizing news articles helps users quickly understand the key points, saving time and improving information retention.

### Importance

This solution is important because it enables:
- **Efficient Information Consumption**: Users get the gist of news articles quickly.
- **Daily Updates**: Automated daily summaries keep users informed without manual effort.
- **Broad Coverage**: Aggregates news from multiple sources for comprehensive coverage.

## High-Level System Design

### Components

1. **Data Collection**: Fetches articles from NewsAPI and web scraping.
2. **Text Preprocessing**: Cleans and prepares the text data.
3. **Text Summarization**: Utilizes machine learning models for extractive and abstractive summarization.
4. **Automation**: Schedules daily summary posting.
5. **Deployment**: Hosts the application and makes it accessible.

### Connections

- **Data Collection** feeds into **Text Preprocessing**.
- **Text Preprocessing** outputs are used by **Text Summarization**.
- **Automation** ensures **Text Summarization** results are posted daily.
- **Deployment** integrates all components and serves the application.

## Detailed Design, Implementation, and Analysis

### Data Collection

- **Sources**: NewsAPI, web scraping (e.g., Reuters, BBC, CNN).
- **Tools**: `requests`, `BeautifulSoup`.

### Text Preprocessing

- **Steps**: Tokenization, stop words removal, normalization.
- **Tools**: `nltk`, `re`.

### Text Summarization

#### Extractive Summarization

- **Approach**: K-Means clustering.
- **Tools**: `scikit-learn`.

#### Abstractive Summarization

- **Model**: `t5-small` from Hugging Face Transformers.
- **Tools**: `transformers`.

### Automation

- **Scheduling**: Using `schedule` library.
- **Daily Posting**: Posts summaries at 8:00 AM every day.

### Deployment

- **GitHub Pages**: For hosting static content.
- **Heroku**: For deploying the Flask backend (if needed).

## Evaluation

### Metrics

- **ROUGE Score**: Evaluates the quality of summaries.
- **User Feedback**: Collects user feedback for improvement.

### Results

- Detailed analysis of the summarization performance.
- Comparison with baseline methods.

## Final Discussion

### Strengths

- **Automation**: Completely automated news summarization and posting.
- **Accuracy**: High-quality summaries using advanced models.
- **Scalability**: Easily scalable to include more news sources.

### Limitations

- **Dependency on External APIs**: Relies on NewsAPI and website structures.
- **Model Limitations**: T5-small may not capture all nuances.

### Recommendations

- **Model Improvement**: Experiment with larger models for better performance.
- **More Sources**: Integrate additional news sources.
- **User Interface**: Develop a more interactive and user-friendly interface.

## How to Deploy

### Using GitHub Pages and Heroku

1. **Create GitHub Repository**:
   - Follow the steps outlined in the previous sections to create and push to a GitHub repository.

2. **Enable GitHub Pages**:
   - Go to the repository settings and enable GitHub Pages.

3. **Deploy on Heroku**:
   - Create a `Procfile` and `requirements.txt`.
   - Follow the Heroku deployment steps.

## How to Use

### Prerequisites

- Python 3.7 or higher
- Required Python libraries (see `requirements.txt`)

### Running Locally

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/news-summarizer.git
   cd news-summarizer
