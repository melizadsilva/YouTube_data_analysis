# YouTube Data Analysis Project

## Overview
Python Project to Scrape YouTube data using YouTube Data API. Using YouTube API, I extracted the data and then load this data into a Python Pandas DataFrame and then analyzed this data. Finally, I built simple visualization from this data using the Python Seaborn library.

This project is a Python-based analysis of YouTube channel data, focusing on extracting and visualizing key metrics like subscriber count, views, and video statistics. The goal was to gain insights into the performance of selected YouTube channels, understand trends, and identify top-performing content.

## Tools Used
- **Python**: The primary programming language used for data extraction and analysis.
- **Google API Client**: Used to interact with the YouTube Data API for web scraping.
- **Pandas**: For data manipulation and analysis.
- **Seaborn**: For creating visualizations of the extracted data.

## Process
### 1. Setting Up YouTube API
- The project started by setting up access to the YouTube Data API using the `google-api-python-client` package.
- The API key was generated from the Google Developer Console and used to authenticate requests.

### 2. Extracting Channel Data
- A function was developed to search for channels by name or handle, retrieve their channel IDs, and store these IDs for further data extraction.
- The `youtube.search().list()` endpoint was utilized to find the channels, and the channel IDs were extracted from the response.

### 3. Fetching Channel Statistics
- With the channel IDs, another function was created to fetch detailed statistics for each channel, including subscriber count, total views, total videos, and the ID of the playlist containing all their uploads.
- The data was stored in a Pandas DataFrame for analysis.

### 4. Data Visualization
- **Bar Charts**: Visualizations were created to compare the channels based on subscriber count, views, and total number of videos. Seaborn was used to plot these comparisons.
- **Top Videos**: A deeper dive was conducted into the content of "Alex The Analyst" by scraping video data from the channel's playlist, analyzing top-performing videos, and visualizing the results.

### 5. Scraping Video Details
- The project further explored video-level data by scraping the video IDs from "Alex The Analyst's" channel using the playlist ID.
- Detailed statistics for each video, including views, likes, comments, and publish date, were collected.
- The video data was then analyzed to identify the top 10 videos based on view count and to examine trends in video uploads over time.

### 6. Analyzing Upload Trends
- The analysis included examining the number of videos published per month to identify patterns in content creation.
- A bar plot was generated to visualize the monthly video upload trends.

## Findings & Insights
- **Subscriber Analysis**: Among the channels analyzed, substantial differences were found in subscriber counts, indicating varying levels of audience reach and engagement.
- **Content Performance**: "Alex The Analyst's" top 10 videos were identified, showing which topics or formats resonated most with the audience.
- **Upload Trends**: The analysis of video uploads per month revealed consistent content creation, which is a key factor in maintaining and growing an audience.

## Conclusion
This project demonstrates how data from YouTube channels can be effectively scraped, analyzed, and visualized using Python. The insights gained can help content creators understand their audience better, optimize their content strategy, and ultimately grow their channels.


