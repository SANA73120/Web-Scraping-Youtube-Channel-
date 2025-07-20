
# 📺 YouTube Video Scraping & Visualization – Yujin-kun Channel
## 📌 Problem Statement

This project helps understand how a YouTube channel performs over time by extracting and analyzing its video data. It uses the YouTube Data API to fetch key information from a YouTube channel — including video titles, views, likes, publish dates, and comment counts.

This data is then visualized on power bi to gain insights like:

- Most viewed videos
- Posting frequency over time
- Correlation between views and likes/comments
- Monthly publishing trends

By analyzing this data, we can help content creators or marketers evaluate what kind of content performs best, when to post videos, and how engagement metrics change over time.

Since Yujin-kun is a gaming YouTuber, this project focuses on identifying the most successful gaming content and how consistently it was published.


### 🪜 Steps Followed

- 📡 YouTube Data API v3
- 🔑 YouTube API Key
- 🐍 Python
- 📁 Pandas
- 📈 Power BI
- 🧪 Jupyter Notebook


### 🪜 Steps Followed
- Step 1: Obtained a YouTube API key from the Google Cloud Console with access to YouTube Data API v3.

- Step 2: Identified the channel ID of Yujin-kun’s YouTube channel.

        Channel ID: UCzrV-4wRCiaVZKRO0YM2AcA

- Step 3: Used Python’s requests library to call the API and extract metadata for all videos, including:

        Video Title
        Video ID
        Publish Date
        View Count
        Like Count
        Comment Count


- Step 4: Stored the data in a Pandas DataFrame and cleaned it by:

        Removing null or incomplete entries
        Converting publish dates to datetime format
        Creating additional calculated columns like Year, Month, and Title Length

- Step 5: Load data into Power BI Desktop, dataset is a escel file.
- Step 6 : Open Power Query Editor and under the View tab in the Data Preview section, enable "Column distribution", "Column quality", and "Column profile" options.
- Step 7 : By default, profiling is done on the first 1000 rows. So, to get a full profile, select “Column profiling based on entire dataset.”
- Step 8: Visual filters (Slicers) were added for fields such as Year to enable dynamic analysis.
- Step 9: Visualizations created included:

        📊 Bar chart of videos uploaded per month
        📈 Line plot showing most viewed videos overtime
        📊 Bar chart of top 10 most viewed videos
        📉 Clustered Column chart for video performance
 
 # Report Snapshot (Power BI DESKTOP)

 <img width="886" height="501" alt="Capture" src="https://github.com/user-attachments/assets/340b18e3-5cf5-4e68-97ea-6a895dd53a81" />


# 📈 Insights

A single page report was created on Power BI Desktop.

Following inferences can be drawn from the dashboard;

        Yujin-kun’s most viewed videos are related to specific gameplay events and titles, indicating what the audience prefers.
        A strong positive correlation was observed between views and likes, and a moderate one with comments, showing that likes are a better indicator of video success.
        Video title length showed a mild impact on views — shorter, focused titles tend to perform better.

# 🌐 Outcome
This project successfully demonstrates how the YouTube Data API can be used for content analysis. It helps uncover patterns in content engagement, publishing strategy, and audience interest.

Such analysis can guide YouTubers, brands, and digital marketers in optimizing content strategy and understanding what drives engagement on YouTube.

