# global_temp
python script to pull temps from openweather map and calculate the global average, also shows hottest and coldest place on the planet. The results can be recorded to a time series database (influxdb) and used to display trends in the global temperature. 

By quickly pulling from 1000s of locations a reasonible average global temperature can be calculated. By running once a day, a daily average can be recorded. I expect some seasonal variation over a year due the more weather stations being in the Northern hemisphere.

usage: global-temp [-h] [--influx INFLUX [INFLUX ...]]
                   [--read READ [READ ...]] [--key KEY [KEY ...]]

optional arguments:
  -h, --help            show this help message and exit
  --influx INFLUX [INFLUX ...]
                        influx server, port, user and password
  --read READ [READ ...]
                        Import stations from json file
  --key KEY [KEY ...]   add an api key, see https://openweathermap.org/api

