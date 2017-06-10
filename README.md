# Value Viz

Documentation for our pricing data.
* [Website](http://quantprice.herokuapp.com)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Daily prices

You need to be familiar with RESTFUL services.

```
https://quantprice.herokuapp.com/api/v1.1/scoop/daily?tickers=MSFT&date=2017-06-10
```

### Historical prices

You have to provide a 

```
https://quantprice.herokuapp.com/api/v1.1/scoop/period?tickers=MSFT&begin=2012-02-19
```

### Multiple tickers

You can just comma separate tickers:

```
https://quantprice.herokuapp.com/api/v1.1/scoop/period?tickers=IBM,MSFT&begin=2012-02-19
```
