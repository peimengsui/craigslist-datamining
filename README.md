# craigslist-datamining

This repo includes works related to mining data from craigslist for understanding neighborhood shopping interests. 

The first part is a scraper implemented with Python Scrapy for getting post titles and link. To run the scraper, please go to the directory of the scrapy project, and run
```{bash}
scrapy crawl craig -o items.csv -t csv
```

This will automatically download the data into .csv file. You can change the webpage you want to scrape in the test.py under directory /spiders. start_urls = ["http://sfbay.craigslist.org/search/npo"] this line allows you to specify the link.

After getting the data, a sample report including for sale post title analysis can be found in the craigslist_title_analysis.ipynb.

