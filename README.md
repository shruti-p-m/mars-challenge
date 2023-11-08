# mars-challenge

This challenge contains two jupyter notebook files: part_1_mars_news.ipynb, and part_2_mars_weather.ipynb. This challenge also contains a mars_temp.csv file which is outputted by part_2_mars_weather.ipynb.

## part_1_mars_news.ipynb
This script visits a Mars News website, and scrapes the title and article preview text of each article on the home page. The script then stores the title and preview text in a dictionary.

## part_2_mars_weather.ipynb
This script visits a Mars Temperature Data website, and scrapes the table on the page. 

This table contains the following information:
- id: the identification number of a single transmission from the Curiosity rover
- terrestrial_date: the date on Earth
- sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
- ls: the solar longitude
- month: the Martian month
- min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
- pressure: The atmospheric pressure at Curiosity's location

The table is then loaded into a pandas dataframe before being analyzed to answer the following questions:
1. How many months exist on Mars?
2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
3. What are the coldest and the warmest months on Mars (at the location of Curiosity)?
4. Which months have the lowest and the highest atmospheric pressure on Mars?
5. About how many terrestrial (Earth) days exist in a Martian year?

   Questions 3-5 have a graphs that accompany the analysis.
   A summary of the answers to questions 3-5 is found after all of the graphs.
   After the analysis, the script then outputs the pandas DataFrame of the table on the Mars Temeperature Data websire into a csv called mars_temp.csv.

## Citations
- the part_2_mars_weather.ipynb script used code from the website: https://saturncloud.io/blog/how-to-add-new-rows-to-a-pandas-dataframe/ to add rows from the table to a the bottom of the dataFrame using the loc function
