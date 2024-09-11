# News Summarizer Application

## Brief Description

The News Summarizer Application is a Python-based tool designed to automate the process of fetching, summarizing, and posting news articles to a WordPress blog. It uses Natural Language Processing (NLP) to generate concise summaries and fetches relevant images to create engaging content.


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
In the digital age, staying informed can be challenging with the overwhelming amount of news content available. The News Summarizer Application simplifies this by providing concise summaries and relevant images of news articles automatically on a WordPress blog.


## Features
- Fetches news articles from multiple sources.
- Generates both extractive and abstractive summaries.
- Fetches relevant images based on the article title.
- Automatically posts summaries to a WordPress blog.
- Runs daily to keep the blog updated with fresh content.


## System Design
The system is designed with the following components:
- **Data Collection Module**: Fetches news articles using APIs and web scraping.
- **Preprocessing Module**: Cleans and preprocesses articles for summarization.
- **Summarization Module**: Generates concise summaries using NLP techniques.
- **Image Fetching Module**: Fetches relevant images from Unsplash.
- **Publishing Module**: Posts summarized content to WordPress.
- **Scheduling Module**: Schedules daily updates to keep the blog fresh.


## Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/stanleymay20/news-summarizer.git

2. **Install dependencies**:
   ```bash
     pip install -r requirements.txt

4. **Set Up Environment Variables**: Create a .env file in the root directory and add API keys:
   ```bash
   NEWS_API_KEY=your_news_api_key
   WORDPRESS_URL=https://your-wordpress-site.com/xmlrpc.php
   WORDPRESS_USERNAME=your_username
   WORDPRESS_PASSWORD=your_password
   UNSPLASH_ACCESS_KEY=your_unsplash_access_key


## Usage
      ```bash
      python app.py


The application will automatically fetch news articles, generate summaries, fetch images, and post them to your WordPress blog.


#### APIs and Environment Setup
News API: Used to fetch news articles. Register at News API to get your API key.
Unsplash API: Used to fetch relevant images. Register at Unsplash Developers to get your access key.
WordPress XML-RPC API: Used to post content on WordPress. Make sure XML-RPC is enabled on your WordPress site.


## Deployment
The project can be deployed on Vercel for continuous deployment. Follow these steps:

1. **Install Vercel CLI**:
   ```bash
   npm install -g vercel

2. Deploy the Project:
   vercel

Follow the prompts to link your GitHub repository and deploy the project.


## Contributing
Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.





