# EasyIP feature

**IP location**
**in development...**

## IP location

**Returns the data structure**

```
{
  "code": 0,
  "msg": "",
  "data": Object
}
```

**code** Status code, 0 for success, other reference error code list.
**msg** Error message
**data** depends on the interface, the same interface will only have one structure.  

## IP location

Interface example

**Request (GET)**

```
http://api.easyapi.link/v1/getIp?secretKey=4b42850e2b30447aacd52479f297cbba&ip=183.11.68.242
```

**Result**

```json
{
  "code": 0,
  "msg": "",
  "data": {
    "ip": "106.133.85.19",
    "lat": 35.6893,
    "lng": 139.6899,
    "countryCode": "JP",
    "countryName": "Japan",
    "region": "Tokyo",
    "city": "Tokyo",
    "operator": "",
    "timezone": "Asia/Tokyo"
  }
}
```

```
ip: indicates the IP address
lat: latitude
lng: longitude
countryCode: indicates the country code
countryName: indicates the country name
region: Province
city: The city.
operator: operator
timezone: indicates the timezone
```

