# GooogelMapAPI
Google Maps get Place API(POST)
This API Will existing place insert to Server
Complete URL https://rahulshettyacademy.com/maps/api/place/add/json? key=qaclick123
Base URL: https://rahulshettyacademy.com/
Resource: /maps/api/place/add/json
Query Parameters: key=qaclick123
Http Method: POST  
Sample Request:
{
  "location": {
    "lat": -38.383494,
    "lng": 33.427362
  },
  "accuracy": 50,
  "name": "Frontline house",
  "phone_number": "(+91) 983 893 3937",
  "address": "29, side layout, cohen 09",
  "types": [
    "shoe park",
    "shop"
  ],
  "website": "http://google.com",
  "language": "French-IN"
}
Sample Response:
{    "status": "OK",
    "place_id": "a0a05095c1de9c8d7a0b6e3017e6fdf8",
    "scope": "APP",
    "reference": "3916bfc5be55899cd111ceecfd5f06663916bfc5be55899cd111ceecfd5f0666",
    "id": "3916bfc5be55899cd111ceecfd5f0666"
}
Google Maps get Place API(GET)
This API Will existing place details from Server
Complete URL https://rahulshettyacademy.com/maps/api/place/get/json?place_id=xxxx&key=qaclick123
Base URL: https://rahulshettyacademy.com/
 Resource: /maps/api/place/get/json
 Query Parameters: key,  place_id ( place_id  value comes from Add place response)
Http Method: GET  
Sample Response:
{
    "location": {
        "latitude": "-38.383494",
        "longitude": "33.427362"
    },
    "accuracy": "50",
    "name": "Frontline house",
    "phone_number": "(+91) 983 893 3937",
    "address": "29, side layout, cohen 09",
    "types": "shoe park,shop",
    "website": "http://google.com",
    "language": "French-IN"
}
Google Maps get Place API(PUT)
This API Will update existing place in Server with new values
Complete URL https://rahulshettyacademy.com/maps/api/place/put/json?place_id=xxxx&key=qaclick123
Base URL: https://rahulshettyacademy.com/
Resource: /maps/api/place/put/json
Query Parameters: key,  place_id ( place_id  value comes from Add place response)
Http Method: PUT
Sample Request:
{
  "place_id":"8d2573bdf6ceec0e474c5f388fa917fb",
  "address":"70 Summer walk, USA",
  "key":"qaclick123"
}

Sample Response:
{
    "msg": "Address successfully updated"
}
Google Maps get Place API(DELETE)
This API Will update existing place in Server with new values
Complete URL https://rahulshettyacademy.com/maps/api/place/delete/json?place_id=xxxx&key=qaclick123
Base URL: https://rahulshettyacademy.com/
Resource: /maps/api/place/delete/json
Query Parameters: key,  place_id ( place_id  value comes from Add place response)
Http Method: DELETE
 Sample Request: 
 Sample Body:
{
    "place_id":" a0a05095c1de9c8d7a0b6e3017e6fdf8"
}

Sample Response:
{
    "status": "OK"
}
