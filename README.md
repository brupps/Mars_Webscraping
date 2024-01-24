# Mars_Weather_Webscraping
The assignment outline below was completed by using webscraping techniques learned in class. In addition, once the data was scraped it was organized into dataframes and then analyzed. Once that was completed the data was exported to a CSV file.

## Skills
- Webscraping
- Splinter
- Pandas
- Beautiful Soup
- Matplotlib

## Results
Through the analysis of the data provided, it was determined that the third Martian month was the coldest with an average temperature of -83.307292ºC while the warmest month was month nine with an average temperature of -69.171642ºC--which in human terms, is incredibly cold. A year on Mars is about 687 days.


## Instructions
Part 1: Scrape Titles and Preview Text from Mars News
Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.
1. Use automated browsing to visit the Mars news site Links to an external site. . Inspect the page to identify which elements to scrape. HINT
2. Create a Beautiful Soup object and use it to extract text elements from the website.
3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
    * Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following: {'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
    *  'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
    * 
    * Store all the dictionaries in a Python list.
    * Print the list in your notebook.
4. Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)
Part 2: Scrape and Analyze Mars Weather Data
Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.
1. Use automated browsing to visit the Mars Temperature Data Site Links to an external site. . Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html. HINT
2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
    * id: the identification number of a single transmission from the Curiosity rover
    * terrestrial_date: the date on Earth
    * sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    * ls: the solar longitude
    * month: the Martian month
    * min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
    * pressure: The atmospheric pressure at Curiosity's location
4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types. HINT
5. Analyze your dataset by using Pandas functions to answer the following questions:
    * How many months exist on Mars?
    * How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    * What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
        * Find the average minimum daily temperature for all of the months.
        * Plot the results as a bar chart.
    * Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
        * Find the average daily atmospheric pressure of all the months.
        * Plot the results as a bar chart.
    * About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
        * Consider how many days elapse on Earth in the time that Mars circles the Sun once.
        * Visually estimate the result by plotting the daily minimum temperature.
6. Export the DataFrame to a CSV file.

## Acknowledgements
I would like to acknowlege my instructor and TAs for their guidance in this project: Othmane Benyoucef, Jacob Peroutek, Isabella Taylor for their guidance and assistance. In addition, I sought out help with code on Stack Overflow and Github.
