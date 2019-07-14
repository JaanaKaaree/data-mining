# data-extraction


## Common required modules
```
pip install pandas
pip install requests
pip install configparser
```


## Social Media



### Facebook

#### Pre requisite 

1. Generate the bearer token
```
https://graph.facebook.com/oauth/access_token
  ?client_id=<your-client-id>
  &client_secret=<your-client-secret>
  &grant_type=client_credentials
```

2. Install facebook modules
```
pip install facebook-sdk
```

#### References
https://developers.facebook.com/docs/places/web/search/
https://developers.facebook.com/docs/graph-api/reference/place-information/


### Google

The **Google Places API** is a great resource for mining data for a giving location. The code in get_google.py will demonstrate the use of this API to retrieve data using the nearbysearch which returns all places in the areas around the passed in geo location coordinates

#### Pre requisite 

1. Get API Key
https://developers.google.com/places/web-service/get-api-key

2. Test your API Key
https://maps.googleapis.com/maps/api/place/nearbysearch/json?location=-33.8670522,151.1957362&radius=500&types=food&name=harbour&key=<API_KEY>

#### References
https://developers.google.com/places/web-service/intro


The code in get_google-images.py retrieves **Google Image Search** results and downloads them into a downloads directory

#### Pre requisite 
1. Install Google images download modules
```
pip install google-images-download
```


### Twitter

