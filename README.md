# f1_crawling

The given code is designed to scrape data from a webpage containing Formula 1 race results for the 2023 season. The code utilizes the `requests` and `BeautifulSoup` libraries to retrieve and parse the HTML content of the webpage.

The code follows these steps:

1. It defines the URL of the webpage that will be scraped.
2. It sends an HTTP GET request to the URL using `requests.get()` and stores the response in the `response` variable.
3. It checks if the response status code is 200 (indicating a successful request).
4. If the status code is 200, it proceeds to extract the data from the webpage using `BeautifulSoup`.
5. It searches for a table element with the class `'resultsarchive-table'` within the parsed HTML content.
6. It finds all row elements (`<tr>`) within the table.
7. It iterates over each row and extracts specific information from the columns.
8. The extracted data, including the position, driver name, nationality, car, and points, is printed.

To save the extracted data to a CSV file, the code can be modified by using the `csv` module. The modified code creates an empty list to store the extracted data, and for each row, it appends the extracted information to a dictionary. It then writes the data to a CSV file using the `csv.DictWriter` class.

By executing the modified code, the extracted data will be saved to a CSV file named "formula1_results.csv" in the same directory as the Python script.
