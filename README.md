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

#### Code and Output
* _Starter Code: Preliminaries_
   ![Screenshot 2025-01-10 at 03 03 34](https://github.com/user-attachments/assets/b84ca052-e708-45bc-a33c-5bcdff3f3bbf)
   ![Screenshot 2025-01-10 at 03 03 43](https://github.com/user-attachments/assets/6d632a81-10d0-4b5e-a7ac-4a4ac6e807d5)

* _Scraping Code: Create a Beautiful Soup_
   ![Screenshot 2025-01-10 at 03 04 00](https://github.com/user-attachments/assets/0585e2d7-f04f-462d-b555-324ba4df23ec)

* _Code to Extract, Store, and Print Results_
   ![Screenshot 2025-01-10 at 03 04 10](https://github.com/user-attachments/assets/bc1f9425-d9f3-4d61-9129-d589a4cef02f)

* _Print Output_
![Screenshot 2025-01-10 at 02 39 50](https://github.com/user-attachments/assets/f7674c2a-fd26-43bb-b247-5838b2af669d)

* _Close Browser_
   ![Screenshot 2025-01-10 at 12 18 24](https://github.com/user-attachments/assets/4222cced-cafd-4020-8f9c-4ac67f6a71cf)

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

#### Code and Output
* _Starter Code: Preliminaries_
   ![Screenshot 2025-01-10 at 12 54 58](https://github.com/user-attachments/assets/36a54c6d-2e6c-4a06-a13e-2c34e3b7a83c)
   ![Screenshot 2025-01-10 at 12 55 10](https://github.com/user-attachments/assets/3db34958-d968-45f1-8352-99297b90981e)

* _Scraping Code: Create a Beautiful Soup and Scrape All Rows of Data_
   ![Screenshot 2025-01-10 at 12 53 26](https://github.com/user-attachments/assets/f0cc1f5a-b58e-4b79-a991-b0f27211a4fe)
   ![Screenshot 2025-01-10 at 12 53 13](https://github.com/user-attachments/assets/e52b801a-b994-4d7a-85dd-1b8d0a082360)

* _Code to Create DataFrame, Examine/Change Data Types_
  ![Screenshot 2025-01-10 at 12 51 37](https://github.com/user-attachments/assets/a26f6ee2-fde6-47cf-a216-3d387d8d0ebe)
  ![Screenshot 2025-01-10 at 12 51 49](https://github.com/user-attachments/assets/cd475092-9876-40ad-a53a-d1104e2261a8)
  
* _Code to Analyze Data and Display Outputs_
  ![Screenshot 2025-01-10 at 12 57 33](https://github.com/user-attachments/assets/3c0132c4-ec4e-49a5-be3a-227474e6a7f4)
   ![Screenshot 2025-01-10 at 12 57 48](https://github.com/user-attachments/assets/f33bb6e0-ed40-4aed-bb31-eb935b2f8856)
   ![Screenshot 2025-01-10 at 12 58 08](https://github.com/user-attachments/assets/1975a789-9fdb-4013-b663-4f03735a4012)
   ![Screenshot 2025-01-10 at 12 58 20](https://github.com/user-attachments/assets/eb054202-1b68-476f-89ec-afa911ed99bc)
   ![Screenshot 2025-01-10 at 12 58 30](https://github.com/user-attachments/assets/e4765688-0565-4f0d-bea9-de7d7d90bfe3)
   ![Screenshot 2025-01-10 at 12 58 42](https://github.com/user-attachments/assets/48a1f039-c275-4638-9361-b54478871fa3)
   ![Screenshot 2025-01-10 at 12 58 50](https://github.com/user-attachments/assets/1a039ade-c2df-4392-ae29-ea10d4e7b894)

* _Code to Report to CSV File and Close Browser_
   ![Screenshot 2025-01-10 at 12 59 06](https://github.com/user-attachments/assets/741b1df5-3c07-4fa1-99bf-0cd8f0038051)

## Acknowledgements

The Mars News website is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from NASA's Mars News website in November 2022. Images are used according to the JPL Image Use Policy, courtesy NASA/JPL-Caltech.
