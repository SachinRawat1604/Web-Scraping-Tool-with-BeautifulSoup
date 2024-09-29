# Web-Scraping-Tool-with-BeautifulSoup
**Purpose:-**
This Python script is designed to scrape data from the Wikipedia page "List of countries and dependencies by population" and save the extracted data in a CSV file.

Prerequisite:-
- Python 3.x installed
- Required libraries:
    - requests
    - BeautifulSoup4
    - csv

**Installation:-**
1. Install required libraries:
   Bash
   pip install requests beautifulsoup4 csv

**Usage:-**
1. Run the script:
   Bash
   python scrape_wikipedia_data.py

**Configuration:-**
1. The target URL for scraping is defined as URL = 'https://en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population'. You can modify this URL to        scrape different Wikipedia pages.
2. The output CSV file is named output.csv by default. You can change this filename in the main function.

**How it works:-**
1. Fetch HTML: The script fetches the HTML content of the target Wikipedia page using the requests library.
2. Parse HTML: The HTML content is parsed using BeautifulSoup to create a structured representation of the page.
3. Extract Data: The script extracts the relevant data from the parsed HTML, focusing on the table containing the country and population information.
4. Save to CSV: The extracted data is saved as a CSV file using the csv library.

**Notes:-**
1. The script assumes that the target data is located in the first table with the class "wikitable". If the table structure changes, you might need to adjust the
   extraction logic.
2. Always respect the terms of service of the website you're scraping.
3. Consider adding error handling to handle potential exceptions like network errors or unexpected HTML structures.

**Example Output:- **

The script will create an output.csv file with the following structure:

Country	          Population
United States	    331,002,651
China	            1,439,323,776
India	            1,380,003,928
...	              ...
