# climate-canada-crawler
A scrapy app that automates data retrieval from the Climate Canada historical weather data tool found [here](http://climate.weather.gc.ca/historical_data/search_historic_data_e.html).

## Example:
  scrapy crawl monthly_weather_spider \
    -a run_from=2019-01-01 \
    -a run_to=2019-01-31 \
    -s FEED_URI=scrapy-weather-data-$(date '+%Y-%m-%d')