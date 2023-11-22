# Data_Scrape
This Python script scrapes the front page of Hacker News (https://news.ycombinator.com/news) to retrieve and display top posts based on votes. It utilizes the requests library for web page retrieval and BeautifulSoup for HTML parsing.
Features:

    Web Scraping: Fetches the HTML content of the Hacker News front page and parses it to extract relevant information.

    Post Filtering: Filters posts based on the number of votes, only including those with a vote count exceeding 99.

    Custom List: Creates a custom list of top posts with titles, links, and vote counts.

    Sorting: Sorts the list of posts based on the number of votes in descending order.

How it Works:

    The script sends a GET request to the Hacker News front page and retrieves the HTML content.
    It uses BeautifulSoup to parse the HTML and extracts the titles and links of the posts along with their corresponding vote counts.
    Posts with vote counts greater than 99 are added to a custom list.
    The list is then sorted based on the number of votes in descending order, creating a curated list of top posts.

Usage:

    Run the script to see a curated list of top posts from the Hacker News front page.


python hacker_news_scraper.py

Example Output:


[
    {'title': 'Example Post 1', 'link': 'https://example.com/post1', 'votes': 150},
    {'title': 'Example Post 2', 'link': 'https://example.com/post2', 'votes': 120},
    ...
]

Note:

This script serves as a tool for quickly accessing and discovering the most popular posts on Hacker News, allowing users to stay informed about trending topics in the tech community.
