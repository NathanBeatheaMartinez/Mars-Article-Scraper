
-----------------------------------------------------------------------------------------------------------
Overview
-----------------------------------------------------------------------------------------------------------

Consists of two technical product containing the following deliverables:

Deliverable 1: Scrape titles and preview text from Mars news articles.
Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

------------------------------------------------------------------------------------------------------------
Part 1: Scrape Titles and Preview Text from Mars News
------------------------------------------------------------------------------------------------------------

Use automated browsing to visit the Mars news site Links to an external site.. Inspect the page to identify which elements to scrape.

Create a Beautiful Soup object and use it to extract text elements from the website.
Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:
{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
Store all the dictionaries in a Python list.
Print the list to the notebook.

--------------------------------------------------------------------------------------------------------------
Part 2: Scrape and Analyze Mars Weather Data
--------------------------------------------------------------------------------------------------------------


Use automated browsing to visit the Mars Temperature Data Site Links to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

Create a Beautiful Soup object and use it to scrape the data in the HTML table.

Assemble the scraped data into a Pandas DataFrame with the following columns:

- terrestrial_date: the date on Earth
- sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
- ls: the solar longitude
- month: the Martian month
- min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
- pressure: The atmospheric pressure at Curiosity's location

Analyze the dataset by using Pandas functions to answer the following questions:

- How many months exist on Mars?
- How many Martian (and not Earth) days worth of data exist in the scraped dataset?
- What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
- Find the average minimum daily temperature for all of the months.
- Plot the results as a bar chart.
- Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
- Find the average daily atmospheric pressure of all the months.
- Plot the results as a bar chart.
- About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
- Visually estimate the result by plotting the daily minimum temperature.


Export the DataFrame to a CSV file.
