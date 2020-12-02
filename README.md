# save-my-car
It's winter in Chicago, and you don't know where you can leave your car parked? We got you. 

### Problem
Chicago has a fairly onerous and unsually series of winter parking bans which trace their historical origin to the [1979 Chicago Blizzard](https://en.wikipedia.org/wiki/1979_Chicago_blizzard)

This is the official info on it:
https://www.chicago.gov/city/en/depts/streets/provdrs/traffic/svcs/winter-snow-parking-restrictions.html

Currently, the city provides this not never descriptive _or_ easy to read map:
https://www.chicago.gov/content/dam/city/depts/streets/supp_info/Snow20112012/Snow20172018/overnightL_120617.pdf

I find the map super hard to read, and haven't seen any media outlets do a better job.

### Background (maybe fill out later)

WBEZ story: http://interactive.wbez.org/towing-the-line/?fbclid=IwAR3RpcBb6GlFJQokoAkHEbkS0VnX-5lle1NI77vbZdMp9i4C1Xjy5I0h8_0

### Solution 

#### Use cases
As a resident, I need an easy and interactive way to tell where I might get towed if I leave my car. 

#### Requirements 

We need data on:
* which street segments are illegal for winter overnight or 2 inch snow parking?
    * Geometry, multiline string
    * a reasonable buffer around those geometries
    * When the restrictions are in effect (bonus)
* where the user wants to park/is parked
    * Lat/Lng Point



### Links, resources


Current city data sources:
https://data.cityofchicago.org/Transportation/Winter-Overnight-Parking-Restrictions/kpim-yiyf
https://data.cityofchicago.org/Transportation/Snow-Route-Parking-Restrictions/i9q6-fx2v

Parsed into GeoJSON:
http://geojson.io/#id=gist:easherma/f4ac5933238aaa732f10e78de656cbf7&map=11/41.8612/-87.6630
http://geojson.io/#id=gist:easherma/58141e8b97fde8baba0db9e2f6c969da&map=11/41.8337/-87.6805
