Database of IPv4 address networks with their respective geographical location.

## Data

Based on GeoLite2 Country Free Downloadable Databases as of Apr 21, 2015 http://dev.maxmind.com/geoip/geoip2/geolite2/

Two files were used to generate this dataset: 

```
GeoLite2-Country-Blocks-IPv4.csv  
GeoLite2-Country-Locations-en.csv  
```

## Preparation

Once a week, a new dataset is automatically downloaded from MaxMind and then processed using a Github Action. The Github Action uses the `geoname_id` column to combine the two CSVs together, to add the country and continent information. If the resulting output has changed, the updated file `data/geoip2-ipv4.csv` is committed.

## License

Datapackage: Creative Commons Zero 

Original CSV: This dataset includes GeoLite2 data created by MaxMind, available from www.maxmind.com
