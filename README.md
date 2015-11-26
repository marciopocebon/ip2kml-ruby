# ip2kml

## Description

Command line program to geolocate IP addresses or domain names
and generate a Google Earth/Map file to visualize locations.

## Installation

```
gem install ip2kml
```

## Command Line Usage

Pipe IP addresses and domain names separated by newlines through
standard input to ip2kml and pipe the output to a kml file.
Open the file in Google Earth or Google Maps

```
cat ip_list.txt | ip2kml > ip_geo.kml
```

## Notes

The free service from www.freegeoip.net is rate limited. It limits you to 10,000
requests per hour. Be mindful of how many IP addresses you are supplying because it
has to perform an HTTP request for each one. This is meant for small numbers of IP
addresses. If you need to do a large amount, you should set up your own local
instance of freegeoip. https://github.com/fiorix/freegeoip

## Contact

nanodano@devdungeon.com

http://www.devdungeon.com

https://github.com/nanodano