# Module 11 Challenge

## <p style="color:#CC6600">Background / Scenario</p> 

You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

As you work on this Challenge, remember that you’re strengthening the same core skills that you’ve been developing until now: collecting data, organizing and storing data, analyzing data, and then visually communicating your insights.
<br>

## <p style="color:#CC6600">Part 1: Scrape Titles and Preview Text from Mars News</p> 

Automated browsing was used to visit the [Mars news site](https://static.bc-edx.com/data/web/mars_news/index.html) and to inspect the page to identify which elements to scrape.

A Beautiful Soup object was created and used to extract text elements (titles and preview text of the news articles) from the website.

The scraped data was then stored in a JSON file to ease sharing the data with others.
<br>

## <p style="color:#CC6600">Part 2: Scrape and Analyze Mars Weather Data</p> 

Automated browsing was used to visit the [Mars temperature data site](https://static.bc-edx.com/data/web/mars_facts/temperature.html) and to inspect the page to identify which elements to scrape.

A Beautiful Soup object was created and used to scrape the data in the HTML table.

The scraped data was assembled into a Pandas DataFrame. The column headings are as follows:
- `id`: the identification number of a single transmission from the Curiosity rover
- `terrestrial_date`: the date on Earth
- `sol`: the number of elapsed sols (Martian days) since Curiosity landed on Mars
- `ls`: the solar longitude
- `month`: the Martian month
- `min_temp`: the minimum temperature, in Celsius, of a single Martian day (sol)
- `pressure`: The atmospheric pressure at Curiosity's location

The dataset was analyzed by using Pandas functions to answer the following questions. See cell outputs in the `part_2_mars_weather.ipynb` file for answers and associated plots.
- How many months exist on Mars?
- How many Martian (and not Earth) days worth of data exist in the scraped dataset?
- What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
    - Find the average minimum daily temperature for all of the months.
    - Plot the results as a bar chart.
- Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
    - Find the average daily atmospheric pressure of all the months.
    - Plot the results as a bar chart.
- About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    - Visually estimate the result by plotting the daily minimum temperature.

The DataFrame was exported to a CSV file.

## <p style="color:#CC6600">References</p>

The [Mars news website](https://static.bc-edx.com/data/web/mars_news/index.html) is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from [NASA's Mars News](https://science.nasa.gov/mars/) website in November 2022. Images are used according to the [JPL Image Use Policy](https://www.jpl.nasa.gov/jpl-image-use-policy), courtesy NASA/JPL-Caltech.
<br>
<br>
<br>
![UTlogo](images/utaustin-mccombs.png)      <img src="images/edx-logo-elm.svg" width="200" height="80"> 