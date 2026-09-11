# News Summarizer Application

> **Historical prototype.** This repository preserves the original 2024 experimental lineage of the News Summarizer project. The structured academic successor is [`text-summarization-news-aggregation`](https://github.com/stanleymay20/text-summarization-news-aggregation). This repository is intentionally retained because `news_summarizer.ipynb` contains unique Reuters scraping, TF-IDF extractive summarization, and Flask trigger experiments that are not currently implemented in the successor. Do not delete this repository as a duplicate.

## Brief Description

The News Summarizer Application is a Python-based prototype designed to automate the process of fetching, summarizing, and posting news articles to a WordPress blog. The notebook explores NewsAPI ingestion, Reuters scraping, extractive and abstractive summarization, WordPress publishing, and a Flask trigger endpoint.

The repository also contains historical environment/deployment artifacts. It should be treated as **prototype/evidence**, not as the current production-ready implementation.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [System Design](#system-design)
- [Installation](#installation)
- [Usage](#usage)
- [APIs and Environment Setup](#apis-and-environment-setup)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Introduction
In the digital age, staying informed can be challenging with the overwhelming amount of news content available. This prototype explored an automated pipeline for collecting news, generating concise summaries, and publishing them to WordPress.

## Features

Experimental work preserved in the repository includes:

- NewsAPI article collection;
- Reuters archive scraping;
- TF-IDF extractive summarization;
- T5-based abstractive summarization;
- WordPress publishing;
- a Flask `/summarize` trigger endpoint.

Earlier documentation also proposed image fetching and scheduled updates. Those claims should be treated as design intent unless corresponding executable source is present; no Unsplash implementation was found in the current notebook.

## System Design
The intended system design included:
- **Data Collection Module**: news APIs and web scraping.
- **Preprocessing Module**: article cleaning and preprocessing.
- **Summarization Module**: extractive and abstractive NLP experiments.
- **Image Fetching Module**: proposed Unsplash integration.
- **Publishing Module**: WordPress publishing.
- **Scheduling Module**: proposed scheduled updates.

### News Summarizer Workflow Diagram

![News Summarizer Workflow](docs/Copy%20of%20News%20summarizer%20workflow%20chart.png)

*Figure 1: News Summarizer Application Workflow*

### Data Flow Diagram

![News Summarizer Data Flow Diagram](docs/Data%20Flow%20Diagram%20for%20News%20Summarizer%20Application%20(5).png)

### Architecture Diagram

![News Summarizer Architecture Diagram](docs/Copy%20of%20Architecture%20Diagram%20for%20News%20Summarizer%20(1).png)

## Installation

This repository is retained primarily for historical/academic evidence. If reproducing the notebook, create a fresh virtual environment rather than using the committed historical `myenv/` directory.

```bash
git clone https://github.com/stanleymay20/news-summarizer.git
cd news-summarizer
python -m venv .venv
pip install -r requirements.txt
```

Create a local `.env` only as needed. Never commit real credentials.

## Usage

The principal executable evidence is the `news_summarizer.ipynb` notebook. The earlier README referred to `app.py`, but no `app.py` exists on the current default branch.

## APIs and Environment Setup

Historical experiments/reference designs use:

- **NewsAPI** for article ingestion;
- **Reuters** archive scraping in the notebook;
- **WordPress** credentials for publishing experiments;
- **Unsplash** only as a proposed/documented image source in the current repository state.

Keep all credentials in environment variables or repository secrets.

## Deployment

Deployment files in this repository are historical evidence and should not be treated as a verified deployment pipeline. Review external publishing side effects and current dependencies before reactivating any automation.

## Contributing

This repository is historical. New implementation work should normally target the structured successor unless it specifically concerns preservation of the prototype lineage.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
