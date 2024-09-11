# Environment Setup Guide

## Step 1: Obtain API Keys
1. **NewsAPI**: Register on [NewsAPI](https://newsapi.org/) and generate your API key.
2. **Unsplash API**: Create an account on [Unsplash](https://unsplash.com/developers) and obtain an access key.
3. **WordPress XML-RPC API**: Ensure XML-RPC is enabled on your WordPress blog. Refer to [WordPress XML-RPC](https://wordpress.org/support/article/xml-rpc/) for more details.

## Step 2: Create a `.env` File
Create a `.env` file in the root directory of your project and add the following:

NEWS_API_KEY=your_news_api_key 

WORDPRESS_URL=https://your-wordpress-site.com/xmlrpc.php 

WORDPRESS_USERNAME=your_username 

WORDPRESS_PASSWORD=your_password 

UNSPLASH_ACCESS_KEY=your_unsplash_access_key





Ensure this file is included in your `.gitignore`.
