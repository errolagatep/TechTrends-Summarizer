TechPulse Digest (AI-Powered Tech News Summarizer)

This project is an automated tech news summarizer built with n8n.
It fetches the latest articles from the Fox News Tech RSS feed, extracts article content, summarizes them using an AI model, and stores the structured insights into Airtable for easy tracking and future use.

🚀 Features

- Automated Fetching – Pulls the latest tech articles from the Fox News Tech RSS feed.

- Content Extraction – Retrieves the full article text via HTTP requests.

- AI Summarization – Uses OpenAI’s Chat Model to generate concise and meaningful summaries.

- Data Transformation – Converts raw HTML to Markdown for cleaner AI input.

- Structured Storage – Saves article details and summaries into Airtable.

- Scalable Workflow – Runs on a schedule with minimal manual intervention.


🛠️ Workflow Overview

1. Schedule Trigger – Defines when the workflow should run.

RSS Read – Fetches the latest tech news articles from:
https://moxie.foxnews.com/google-publisher/tech.xml

2. Limit Node – Controls how many articles are processed per run.

3. HTTP Request – Fetches the full article body.

4. Markdown Conversion – Transforms HTML into Markdown for better readability.

5. AI Summarizer (OpenAI) – Generates a short, meaningful summary of the article.

6. Edit Fields – Cleans and structures the extracted data.

7. Airtable Integration – Stores the article title, link, and AI summary in a database.


⚡ Tech Stack

- n8n – Workflow automation tool.

- OpenAI – AI-powered text summarization.

- Airtable – Storage and database for summarized articles.

- Fox News Tech RSS Feed – Source of articles.