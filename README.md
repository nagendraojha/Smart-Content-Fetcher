# Smart-Content-Fetcher
Here is a description for the README file for your GitHub project:

---

# Smart Content Fetcher

The **Smart Content Fetcher** is a Python-based application that allows users to search for topics and retrieve verified content, Wikipedia summaries, or full content from various online sources. The application features an intuitive GUI built using **Tkinter** and supports multiple search options, including Wikipedia summaries, verified information from various sources, and full content scraped from the web.

### Key Features:

- **Search Interface**: Users can easily enter a search term and retrieve relevant information.
- **Multiple Content Sources**: The application fetches content from multiple sources such as Wikipedia and verified web results.
- **Verified Information**: It cross-references data from Wikipedia and other web sources to provide more accurate and reliable content.
- **Real-time Web Search**: Users can search the web directly from the application for additional information.
- **Text Results**: The results are displayed in a text area with scrollbars and a progress bar for loading status.
- **Content Combination**: The application intelligently combines content from multiple sources to provide the most comprehensive answer.
- **Web Scraping**: It scrapes content from web pages using the BeautifulSoup library and filters out unwanted elements.

### Libraries Used:

- **wikipedia**: To fetch summaries and full content from Wikipedia.
- **requests**: For making HTTP requests to fetch web content.
- **Tkinter**: To create the GUI for the application.
- **BeautifulSoup**: For scraping and cleaning web pages.
- **googlesearch**: To perform a Google search and get top relevant URLs.
- **concurrent.futures**: For running multiple tasks concurrently to speed up data fetching.

### Installation:

To install the necessary libraries, run:

```bash
pip install wikipedia requests beautifulsoup4 googlesearch-python
```

### Usage:

1. **Search for a Topic**: Enter a search term in the search box and choose the type of content you want to fetch (Verified Summary, Wikipedia Summary, or Full Content).
2. **View Results**: The content will be displayed in the result section of the GUI, with a progress bar showing the search status.
3. **Search Web**: You can open a browser tab to search the topic on Google directly.
4. **Clear Results**: You can clear the results at any time.

### Code Overview:

- **ContentFetcher Class**: Manages the GUI and content fetching logic. It handles search input, content fetching from various sources, and displays the results.
- **Fetching Methods**: Methods like `get_verified_content`, `get_wikipedia_summary`, and `get_full_content` fetch data from different sources. 
- **Scraping**: The `scrape_website` method uses BeautifulSoup to extract useful content from web pages.
- **Concurrency**: The app uses `concurrent.futures.ThreadPoolExecutor` to fetch content concurrently, improving performance.

### Example Screenshot:
<img width="673" alt="smart_search" src="https://github.com/user-attachments/assets/dfc1b22b-f3a9-4d70-875b-4e4ec95c0dbf" />


---

