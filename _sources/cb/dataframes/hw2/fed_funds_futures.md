# Dataframe: `hw2:fed_funds_futures` - 30-Day Fed Funds Futures

Daily OHLCV bars (ohlcv-1d schema) from the CME Globex dataset (GLBX.MDP3), pulled with parent symbology (ZQ.FUT) so one request returns every listed ZQ contract. Columns: date (tz-naive trading date), symbol, open, high, low, close, volume. A contract settles at 100 minus the calendar-day average effective federal funds rate over its month, so 100 - close is the market's forecast of that average rate. The symbol column also holds calendar spreads such as ZQU6-ZQZ6; keep only outright contracts such as ZQU6 (fedwatch.filter_outright_contracts) before using prices. Contracts far from expiry trade thinly and can miss days.


## DataFrame Glimpse

```
Rows: 11744
Columns: 7
$ date   <datetime[ns]> 2026-10-20 00:00:00
$ symbol          <str> 'ZQ:BF J7-K7-N7'
$ open            <f64> -1.5
$ high            <f64> -1.5
$ low             <f64> -1.5
$ close           <f64> -1.5
$ volume          <u64> 4


```

## Dataframe Manifest

| Dataframe Name                 | 30-Day Fed Funds Futures                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [fed_funds_futures](../dataframes/hw2/fed_funds_futures.md)                                       |
| Sources                        | CME Group                                          |
| Providers                      | Databento                                        |
| Provider Links                 | https://databento.com/                                   |
| Tags                           | Monetary Policy, Futures, Fed Funds                                             |
| Access Types                   |                                       |
| How is data pulled?            | Databento Python client                                                   |
| Data available up to (min)     | 2026-10-20 00:00:00                                                             |
| Data available up to (max)     | 2026-10-20 00:00:00                                                             |
| Dataframe Path                 | /Users/fernandoperezmillan/Desktop/hw2-ferpmillan/_data/fed_funds_futures.parquet                                             |


**Linked Charts:**


- [hw2:fedwatch_latest_forecast](../../charts/hw2.fedwatch_latest_forecast.md)



## Pipeline Manifest

| Pipeline Name                   | HW 2: The Yield Curve and the Policy Path                       |
|---------------------------------|--------------------------------------------------------|
| Pipeline ID                     | [hw2](../../../index.md)              |
| Maintainer                      | Jeremiah Bejarano               |
| Contributors                    | Jeremiah Bejarano |
| Repository                     | https://github.com/hw-finm-32800/hw2                  |
| Pipeline Web Page               | <a href="file:///Users/fernandoperezmillan/Desktop/hw2-ferpmillan/docs/index.html">Pipeline Web Page      |
| Date of Last Code Update        | 2026-10-22 01:45:56           |
| OS Compatibility                | Windows, Linux, macOS |
| Linked Dataframes               |  [hw2:crsp_treasury_consolidated](../../dataframes/hw2/crsp_treasury_consolidated.md)<br>  [hw2:fed_yield_curve](../../dataframes/hw2/fed_yield_curve.md)<br>  [hw2:fed_funds_futures](../../dataframes/hw2/fed_funds_futures.md)<br>  |


**Build Commands:**
```
doit

```

