# LogoExtraction
Python Code 

This program use scrapy package to parse a website for logo extraction.
The name of spider to perform logo extraction is : logo

#Method Detail

This program only process <div>, <a> and <img> tag in order to extract logo.
There are three case to extract logo:

### Case 1: when <a> contains <img> with logo substring in its @src

### Case 2: when <div> contains <img>  with logo substring in its @src

### Case 3: when <a> contains @href as home page address or index. and <img> with possible file extension as like (.png, .gif, .jpg etc) and logo substring in its @class or @title or @alt


# Limitation
1 - This program don't process CSS (style sheet) to parse for LogoExtraction
2 - This program don't process HTML pages having only <Table> instead of <div> for Logo Extraction.
        
# Run
In order to run this program. you can use following command at terminal inside LogoExtraction project
> scrapy crawl logo 

#Output
It will extract the logo url and web page url and save in csv file.
