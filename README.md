# Data Collection Challenge

## Instructions

### Part 1 - Scrape Titles and Preview Text from Mars News

Using Jupyter Notebook, open the starter code part_1_mars_news.ipynb and follow the steps below to scrape the Mars News website. 
1. Use automated browsing to visit the Mars news site. Inspect the page to identify which elements to scrape.
2. Create a Beautiful Soup object, to extract text elements from the website.
3. Extract the title and preview text of the scraped news articles.
    * Store each title-preview pair in a Python dictionary and give each dictionary two keys: title and preview. An example:
    ```
    {'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
     'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae  simultaneously, the result of solar storms that began on Aug. 27."}
    ```
    * Store all the dictionaries in a Python list.
    * Print the list in your notebook.

_Starter Code: Preliminaries_
   ![Screenshot 2025-01-10 at 03 03 34](https://github.com/user-attachments/assets/b84ca052-e708-45bc-a33c-5bcdff3f3bbf)
   ![Screenshot 2025-01-10 at 03 03 43](https://github.com/user-attachments/assets/6d632a81-10d0-4b5e-a7ac-4a4ac6e807d5)

_Scraping Code: Create a Beautiful Soup_
   ![Screenshot 2025-01-10 at 03 04 00](https://github.com/user-attachments/assets/0585e2d7-f04f-462d-b555-324ba4df23ec)

_Code to Extract, Store, and Print Results_
   ![Screenshot 2025-01-10 at 03 04 10](https://github.com/user-attachments/assets/bc1f9425-d9f3-4d61-9129-d589a4cef02f)

_Print Output_
![Screenshot 2025-01-10 at 02 39 50](https://github.com/user-attachments/assets/f7674c2a-fd26-43bb-b247-5838b2af669d)








### Part 2 - Scrape and Analyze Mars Weather Data

Using Jupyter Notebook, open starter code part_2_mars_weather.ipynb and follow the steps below to scrape and analyze Mars weather data.
1. Use automated browsing to visit the Mars Temperature Data Site Links to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.
2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
    * id: the identification number of a single transmission from the Curiosity rover
    * terrestrial_date: the date on Earth
    * sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    * ls: the solar longitude
    * month: the Martian month
    * min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
    * pressure: The atmospheric pressure at Curiosity's location
4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
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
      * Visually estimate the result by plotting the daily minimum temperature of each observation.
6. Export the DataFrame to a CSV file.



## Acknowledgements

The Mars News website is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from NASA's Mars News website in November 2022. Images are used according to the JPL Image Use Policy, courtesy NASA/JPL-Caltech.
