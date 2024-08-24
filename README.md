This Python script is designed for web scraping book information from the "Books to Scrape" website. It uses the requests library to fetch the webpage and BeautifulSoup to parse the HTML content. The script extracts details such as book titles, prices, and availability statuses.

Key Components
scrape_books_to_scrape(url): This function takes a URL as input and sends an HTTP GET request to retrieve the page content. It then parses the HTML using BeautifulSoup, searches for book entries, and extracts the title, price, and availability for each book. The collected data is stored in a list of dictionaries.

main(): This function defines the target URL, calls the scrape_books_to_scrape function to get the book data, and converts the data into a pandas DataFrame. The DataFrame is then saved as a CSV file named books_to_scrape.csv, and a confirmation message is printed.

How It Works
Fetching Data: The script sends a request to the "Books to Scrape" website to retrieve the HTML content.
Parsing HTML: BeautifulSoup is used to parse the HTML and locate relevant data.
Extracting Information: The script finds book titles, prices, and availability statuses within HTML elements and collects this information.
Saving Data: The data is saved into a CSV file for easy access and further analysis.
Usage
To use the script, clone the repository, install the required libraries, and run the script. The output will be a CSV file containing the scraped book details.
