![RAW Labs](https://avatars.githubusercontent.com/u/11390046?s=100&v=4)
# Example Data Products






The following are data products examples built using RAW. More detail and the code is available within these sub-directories<p>
  
Clicking on these endpoints will generally return JSON data into the browser. This is not formatted in most web browsers. Therefore in Chrome, we suggest you install a Chrome extension: JSON formatter - [get from Chrome Webstore](https://chrome.google.com/webstore/search/json%20formatter)
<br>In Safari you can install an extension [like this one](https://apps.apple.com/gb/app/prettyjson-for-safari/id1445328303?mt=12)<br>
  
Comments and suggestions are welcome: feel free to file GitHub Issues or email us at hello@raw-labs.com

* [Movies](#movies)
* [Olympic Games](#olympic-games)
* [ISS](#iss)
* [Weather](#weather)
* [Value at Risk](#value-at-risk)
* [New York Transit](#new-york-transit)
* [RSS news analysis](#rss-news-analysis)
* [Wikipedia](#wikipedia)
* [Emissions](#emissions)
* [Twitter](#twitter)
* [US government](#us-government)
* [SEO](#SEO)

Read our Blogs and Tutorials, many of which are relevant to these examples:
https://www.raw-labs.com/blog
  
See our Docs and Developer Resources:
https://docs.raw-labs.com

Follow us on on Twitter:
https://twitter.com/raw_labs

## [Movies](./1/public/movies)

Endpoints to query data from a copy of the Wikipedia's movie dataset, stored on GitHub.

Movies can be queried by title<p>https://api.raw-labs.com/examples/1/public/movies/movies-by-title?title=river 

or by year<p>https://api.raw-labs.com/examples/1/public/movies/movies-by-year?year=2000

## [Olympic Games](./1/public/olympic-games)

Endpoints combine "open" data hosted on DataHub, as well as files stored on an S3 bucket.

Medals per country<p>https://api.raw-labs.com/examples/1/public/olympic-games/country-medals?country_name=Germany

Medals per athlete (there's a [video](https://www.youtube.com/watch?v=zgBW5kHK-Vo) about this endpoint)<p>https://api.raw-labs.com/examples/1/public/olympic-games/athlete-data?athlete_name=BURKE,%20Thomas

Gold medals per country<p>https://api.raw-labs.com/examples/1/public/olympic-games/country-gold-medals?country_name=Germany

## [ISS](./1/public/ISS)
  
Example showing simple API integration, joining two APIs to produce a third
This example shows the location of the ISS (space station) location, now:
  
https://api.raw-labs.com/examples/1/public/ISS/isslocation

https://api.raw-labs.com/examples/1/public/ISS/isslocationosm
  
  
## [Weather](./1/public/weather)
  Layering on top of a weather provider, in this case visualcrossing.com<br>
  Note these are protected from public access due to licensed data being used. Please contact us at hello@raw-labs.com 

Daily History:
  https://api.raw-labs.com/examples/1/public/weather/history-daily?location=london&yearmonth=2022-01

Hourly History:
  https://api.raw-labs.com/examples/1/public/weather/history-hourly?location=london&yearmonth=2022-01

 
## [Value at Risk](./1/public/value-at-risk)
  
Example showing resource-intensive data products involving calculations on sizeable data:

https://api.raw-labs.com/examples/1/public/value-at-risk/index-var?index=^DJI - Dow Jones 30 stocks

https://api.raw-labs.com/examples/1/public/value-at-risk/index-var?index=^GSPC - S&P 500 stocks

https://api.raw-labs.com/examples/1/public/value-at-risk/index-var?index=^IXIC - Nasdaq 100 stocks

## [New York Transit](./1/public/nyc/mass-transit)
  
Our good friend the New York TLC data set, we show how to query with RAW, and adding MTA data too:
  
https://api.raw-labs.com/examples/1/public/nyc-transit/trips?yearmonth=2021-07
  
More functions, adding Weather data too, note these are protected from public access due to licensed data being used.<br>
Please contact us at hello@raw-labs.com for more information 
  
https://api.raw-labs.com/examples/1/public/nyc-transit/trips-summary-daily-weather?yearmonth=2021-01
  
https://api.raw-labs.com/examples/1/public/nyc-transit/taxi-trips-hourly-weather?yearmonth=2021-01

## [RSS news analysis](./1/public/RSS-analysis)
  
  Analytics on News web pages, including metadata extraction using opengraph.io and entity analytics using Google's natural language API
  
  **CNN US Edition**<br>
RSS:<br>
http://rss.cnn.com/rss/money_news_international.rss<br>
RAW Endpoint:<br>
https://api.raw-labs.com/examples/1/public/RSS-analysis/rss-analysis?url=http://rss.cnn.com/rss/edition_world.rss<br>

  **Huffington Post:**<br>
RSS:<br>
https://www.huffpost.com/section/front-page/feed?x=1 <br>
RAW Endpoint:<br>
https://api.raw-labs.com/examples/1/public/RSS-analysis/rss-analysis?url=https%3A%2F%2Fwww.huffpost.com%2Fsection%2Ffront-page%2Ffeed%3Fx%3D1<br>

**Techcrunch:**<br>
RSS:<br>
https://techcrunch.com/feed/?guccounter=1<br>
RAW Endpoint:<br>
https://api.raw-labs.com/examples/1/public/RSS-analysis/rss-analysis?url=https%3A%2F%2Ftechcrunch.com%2Ffeed%2F%3Fguccounter%3D1<br>

## [Wikipedia](./1/public/wikipedia)
  
  SPARQL queries onto wikidata.org (wikipedia's knowledge graph database)<br>
  
**Heads of Government with Twitter accounts**<br>
https://api.raw-labs.com/examples/1/public/wikipedia/heads-of-government

## [Emissions](./1/public/emissions)
  
 CO2 emissions, US, vs. Rest of World, by year (data from FRED and OWID)<br>
  
**US vs Global CO2 Emissions, by Year**<br>
https://api.raw-labs.com/examples/1/public/emissions/us-vs-global-co2


## [Twitter](./1/public/twitter)

**Recent Tweets**
   Returns the last X tweets from a number of twitter accounts, optionally can use keywords to filter on

https://api.raw-labs.com/examples/1/public/twitter/recent-tweets?twitterName=BorisJohnson<br>
https://api.raw-labs.com/examples/1/public/twitter/recent-tweets?twitterName=POTUS&keywordList=job,jobs,economy,employment

**Heads of Government Tweets**
    Uses Country and Head of Government information queried from Wikipedia, to find the Twitter accounts - then returns the Recent Tweets from those leaders
    
https://api.raw-labs.com/examples/1/public/twitter/heads-of-govt-tweets?countries=France,Germany,Ukraine,United%20Kingdom

## [US Government](./1/public/us-government)
  
  Free open data from https://theunitedstates.io - simple queries used for our [video tutorials](https://raw-labs.com/library/type/videos/)

**US Legislators (current)**

  List of current US Legislators - optional parameters to filter include type, state, party
  
  https://api.raw-labs.com/examples/1/public/us-government/legislators - returns all<br>
  https://api.raw-labs.com/examples/1/public/us-government/legislators?state=CA&type=rep&party=Democrat - Californian, Democrats in House of Representatives

**Sentiment Analysis on Tweets from US Legislators**

  Returns Recent tweets from Twitter, and runs Google Sentiment Analysis on the content of those tweets. 
  Output structure is the raw form from Googles Language API. 

  https://api.raw-labs.com/examples/1/public/us-government/legislators-tweets-sentiment?state=CA&keywordList=job,jobs,employment,economy<br>
  https://api.raw-labs.com/examples/1/public/us-government/legislators-tweets-sentiment?state=NY,NJ&type=sen
  
**Summaries (current & historical)**
  
  summaries of male to female legislators across all current and historical data. 
  These are good examples of union'ing two data structures, creating a summary function as a re-usable intermediate dataset.
  
  https://api.raw-labs.com/examples/1/public/us-government/summary/by-state?states_list=CA,NV<br>
  https://api.raw-labs.com/examples/1/public/us-government/summary/by-party-house?party=Democrat
  
## [SEO](./1/public/SEO)
  
**Historical Search Volume for Google Searches:**

  Endpoint returns Historical Searches for Keywords on Google, by Month.
    
  Note this API uses DataForSEO as a source API, see: https://docs.dataforseo.com/v3/keywords_data/google_ads/search_volume/live/ for more details
     
  https://api.raw-labs.com/examples/1/public/SEO/historical-search-vol?keywords=tesla,bmw&language_code=en&location_name=United%20States
  
  


