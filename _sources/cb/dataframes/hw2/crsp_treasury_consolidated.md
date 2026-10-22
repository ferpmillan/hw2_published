# Dataframe: `hw2:crsp_treasury_consolidated` - CRSP Treasury Consolidated

Consolidated CRSP US Treasury database combining daily pricing data (prices, yields, durations) with issue-level characteristics (coupon, maturity, issue date). Sourced from WRDS.


## DataFrame Glimpse

```
Rows: 2530592
Columns: 20
$ kytreasno                  <f64> 200675.0
$ kycrspid                   <str> '19700815.104000'
$ tcusip                     <str> '912810AG'
$ caldt             <datetime[ns]> 1970-01-02 00:00:00
$ tdatdt            <datetime[ns]> 1963-06-20 00:00:00
$ tmatdt            <datetime[ns]> 1970-08-15 00:00:00
$ tfcaldt                    <i64> 0
$ tdbid                      <f64> 97.34375
$ tdask                      <f64> 97.46875
$ tdaccint                   <f64> 1.5217391304348
$ tdyld                      <f64> 0.0002257801889589
$ price                      <f64> 98.9279891304348
$ tcouprt                    <f64> 4.0
$ itype                      <f64> 1.0
$ original_maturity          <f64> 7.0
$ years_to_maturity          <f64> 1.0
$ tdduratn                   <f64> 221.37694468124
$ tdretnua                   <f64> 0.00085224539168923
$ days_to_maturity           <i64> 225
$ callable                  <bool> False


```

## Dataframe Manifest

| Dataframe Name                 | CRSP Treasury Consolidated                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [crsp_treasury_consolidated](../dataframes/hw2/crsp_treasury_consolidated.md)                                       |
| Sources                        | CRSP                                          |
| Providers                      | WRDS                                        |
| Provider Links                 | https://wrds-www.wharton.upenn.edu/                                   |
| Tags                           | Treasury, Fixed Income, Yield Curve                                             |
| Access Types                   |                                       |
| How is data pulled?            | WRDS via Python                                                   |
| Data available up to (min)     | N/A (large file)                                                             |
| Data available up to (max)     | N/A (large file)                                                             |
| Dataframe Path                 | /Users/fernandoperezmillan/Desktop/hw2-ferpmillan/_data/TFZ_consolidated.parquet                                             |


**Linked Charts:**

- None


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

