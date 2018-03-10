# SwachBharatbot
This is a Scrapy Project to scrape state level,district level,ward level,ulb level data of INDIVIDUAL HOUSEHOLD LATRINE(IHHL) APPLICATION( ﻿http://swachhbharaturban.gov.in/ihhl/RPTApplicationSummary.aspx﻿).
This project is only meant for educational purposes.
## Extracted data
This project extracts the tables present at the mentioned site iteratively.The extracted data is looks like this sample(KEY,PAIR):

OrderedDict([(u'State', u'Andaman & Nicobar Islands'), (u'No. of Applications Received', u'12'), (u'No. of Applications Not Verified', u'9'), (u'No. of Applications Verified', u'0'), (u'No. of Applications Approved', u'0'), (u'No. of Applications Approved having Aadhar No.', u'0'), (u'No. of Applications Rejected', u'0'), (u'No. of Applications Pullback', u'0'), (u'No. of Applications Closed', u'3'), (u'No. of Constructed Toilet Photo', u'0'), (u'No. of Commenced Toilet Photo', u'0'), (u'No. of Constructed Toilet Photo through Swachhalaya', u'46')])


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
