# SwachBharatbot
This is a Scrapy Project to scrape state level,district level,ward level,ulb level data of INDIVIDUAL HOUSEHOLD LATRINE(IHHL) APPLICATION( ﻿http://swachhbharaturban.gov.in/ihhl/RPTApplicationSummary.aspx﻿).
This project is only meant for educational purposes.
## Extracted data
This project extracts the tables present at the mentioned site iteratively.The extracted data is looks like this sample(KEY,PAIR):

{
"No. of Applications Closed": "3", "No. of Applications Rejected": "0", "No. of Applications Pullback": "0", "No. of Commenced Toilet Photo": "0", "No. of Applications Not Verified": "9", "No. of Applications Verified": "0", "State": "Andaman & Nicobar Islands", "No. of Applications Received": "12", "No. of Applications Approved having Aadhar No.": "0", "No. of Constructed Toilet Photo": "0", "No. of Applications Approved": "0", "No. of Constructed Toilet Photo through Swachhalaya": "46"},
{"No. of Applications Closed": "180034", "No. of Applications Rejected": "0", "No. of Applications Pullback": "30", "No. of Commenced Toilet Photo": "25", "No. of Applications Not Verified": "15766", "No. of Applications Verified": "192514", "State": "Andhra Pradesh", "No. of Applications Received": "388344", "No. of Applications Approved having Aadhar No.": "192331", "No. of Constructed Toilet Photo": "192887", "No. of Applications Approved": "192508", "No. of Constructed Toilet Photo through Swachhalaya": "39"
}


## Spiders

This project contains two spiders and you can list them using the `list`
command:

    $ scrapy list
        districtlevelbot
        statelevelbot
        ulblevelbot
        wardlevelbot
districtlevelbot extracts the districtlevel data similarly for others.

You can learn more about the spiders by going through the
[Scrapy Tutorial](http://doc.scrapy.org/en/latest/intro/tutorial.html).


## Running the spiders

You can run a spider using the `scrapy crawl` command, such as:

    $ scrapy crawl districtlevelbot
    
this will generate raw html file

If you want to save the scraped data to a file, you can pass the `-o` option:

    $ scrapy crawl districtlevelbot -o quotes.json
    $ scrapy crawl statelevelbot -o quotes.csv
        




`
