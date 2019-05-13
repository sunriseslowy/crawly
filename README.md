# Crawly

**Commands**

1. Start crawler:
`Crawly.EngineSup.start_spider(BlogEsl)`

** API **

1. Start crawler:
curl -v localhost:4001/spiders/<SpiderName>/schedule
2. Stop crawler
curl -v localhost:4001/spiders/<SpiderName>/schedule
3. Scheduled requests:
curl -v localhost:4001/spiders/BlogEsl/scheduled-requests
4. Scraped Items:
curl -v localhost:4001/spiders/BlogEsl/scraped-items

**Tasks**

***General***
Listen to robots.txt
Throttle
Stopspider signal
Read parameters from settings...

***URL storage***
1. Persistant fingerprints for duplicates filtering...
2. Migrate fingerprints to maps

***Data storage***
1. Define url id field;
2. Store id in data_store state (as map)
3. Pass the worker state to pipeline;
4. Do filtering
5. Update state...

*** Request middlewares ***
1. Filter out requests for other domains +
2. Filter out requests via robots.txt
3. User agent rotation middleware

1. How to close fd?

3. Support -o option to pipe data filename
Item definition
Pipelines