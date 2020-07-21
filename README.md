# Webscrapping-IMDB

The analysis is based on the first 150 most voted on feature films for 2019 on IMDB .
I decided to use web-scrapping as my data collection technique, to ensure the reliability and consistency of the data. 
To do so, I used python, using a third-party library named ‘requests’. I sent a HTTP request to the URL of the IMDB webpage,
the server responding with the HTML content of the webpage. I proceeded to parse the data, however since most of it is nested,
I resorted to a few string processing techniques. I used another third-party python library, Beautiful Soup, to create a data 
tree and parse through it, able to pull out the pieces of information that were of importance for the analysis.
From there, I used the ‘find_all’ function, to separate the html content that referred to each specific movie and continued 
pulling out data from each section. I was able to do so due to the consistency of the html code. I exported that to an excel 
sheet and then to a csv, to more easily process the information in R. 

