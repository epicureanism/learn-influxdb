# What's InfluxDB
> InfluxDB is a database that has been optimized for time series data. 
> This data commonly comes from sources like distributed sensor groups, click data from large websites, or lists of financial transactions.
> - [why-influxdb-isn-t-crud](https://docs.influxdata.com/influxdb/v1.7/concepts/crosswalk/#a-note-on-why-influxdb-isn-t-crud)

# Run in docker
```sh
docker run -p 8086:8086 -d -v influxdb:/var/lib/influxdb influxdb
```
* the docker image exposes the shared volume under /var/lib/influxdb and mount the host directory of "influxdb" to that point.
  ```sh
  -v influxdb:/var/lib/influxdb 
  ```
