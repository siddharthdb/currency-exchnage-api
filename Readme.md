# Currency Exchange Rates API 

Currency Exchnage Rates API is a free service for current and historical foreign exchange rates [published by the European Central Bank](https://www.ecb.europa.eu/stats/policy_and_exchange_rates/euro_reference_exchange_rates/html/index.en.html).

## Local Installation and Execution steps

- Run `pipenv shell`
- Run `pipenv run`

#### Lates & specific date rates
Get the latest foreign exchange rates.

```http
GET /latest
```

Get historical rates for 4 Jan 1999.

```http
GET /2020-08-26
```

## Comming Soon
Rates are quoted against the Euro by default. Quote against a different currency by setting the base parameter in your request.

```http
GET /latest?base=USD
```

Request specific exchange rates by setting the symbols parameter.

```http
GET /latest?symbols=USD,GBP
```

Get exchange rate using a different base currency

```http
GET /2020-08-26?base=USD
```