# Value Viz

Documentation for our pricing data.
* [Website](http://quantprice.herokuapp.com)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Daily prices

You need to be familiar with RESTFUL services.

```
https://quantprice.herokuapp.com/api/v1.1/scoop/day?tickers=MSFT&date=2017-06-09
```
Price data is split adjusted.

### Historical prices

You have to provide a date range :

```
https://quantprice.herokuapp.com/api/v1.1/scoop/period?tickers=MSFT&begin=2012-02-19&end=2012-02-20
```

If you don't provide begin or end it will use the earliest or current date:

```
https://quantprice.herokuapp.com/api/v1.1/scoop/period?tickers=MSFT&begin=2012-02-19
```

Price data is split adjusted.

### Multiple tickers

You can just comma separate tickers:

```
https://quantprice.herokuapp.com/api/v1.1/scoop/period?tickers=IBM,MSFT&begin=2012-02-19
```
Price data is split adjusted.

### Experimantal NASDAQ prices
This contains also ETFS

```
https://nasdaqviz.herokuapp.com/api/v1.1/markets/data/nasdaq/VOO
```

Price data is split adjusted.

### Market trading times

If you want to know what is the status for the NSDAQ and NYSE trading times:

```
https://nasdaqviz.herokuapp.com/api/v1.1/markets/time/NASDAQ
https://nasdaqviz.herokuapp.com/api/v1.1/markets/time/NYSE
```
It takes into account holidays as well.

For NASDAQ will return: Pre Market Open, Regular Open, After Market Open, Closed
For NYSE will return: Open Session, Coret Trading Open, Extended Hours, Closed

### Rate limit

All requests are rate limited to 10 requests per hour.
If you want to register for a full access API send me an email to investment [AT] robomotic [dot] com .
You will receive an API key to add to the URL.

We are setting up a paypal account for paid subscription without rates.

### List of tickers available

https://github.com/robomotic/valueviz/blob/master/scoop_tickers.csv

