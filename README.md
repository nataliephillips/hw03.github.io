# HW 03 WebScraping
### Link to Instructions: [**instructions!!!** ](https://github.com/mikeizbicki/cmc-csci040/tree/2021fall/hw_03)

## What Am I Doing? (she said to herself)
For this homework, I am scraping information from ebay and storing the results in a json and csv files.
To start, I added in command items to be able to choose which ebay web pages that I opened and scraped information from. I defined what I wanted to search, how many pages of the search I wanted and how I would display the information. I then looped over the specified number of webpages to get each items name, price, status, shipping cost, return value and number of items sold. Once extracted, I inputted those values into a json list of libraries to keep everything organized. It downloads the first 10 pages of a specific search term from ebay.

## How to Run the Program
To run the program you need to specify commands in terminal (search term, num_pages, csv)
``` 
python3 ebay_dl.py "search term" "--num_pages= "(default 10) "--csv" (default json)
```

specifying search terms:
``` 
python3 ebay_dl.py hammer 
```
or more than one word search terms:
``` 
python3 ebay_dl.py "stuffed animal" 
```

the default number of pages is 10, so you don't have to specify anything for the ten pages
specifying number of pages: 
```
python3 ebay_dl.py hammer --num_pages=1
```

the default ouput file is json, so you don't have to specify anything for json
to change to csv: 
``` 
python3 ebay_dl.py hammer --csv
```

all the json and csv files in my repository:

hammer json 
``` 
python3 ebay_dl.py hammer
```

hammer csv
``` 
python3 ebay_dl.py hammer --csv
```

stuffed animal json
``` 
python3 ebay_dl.py 'stuffed animal' 
```

stuffed animal csv
``` 
python3 ebay_dl.py 'stuffed animal' --csv
```

cat json
``` 
python3 ebay_dl.py cat
```

cat csv
``` 
python3 ebay_dl.py cat --csv 
```
