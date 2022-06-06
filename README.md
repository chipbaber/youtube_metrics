# API Calls for Getting Youtube Metrics
Below is code and notes to access youtube video metrics.

- API Documentation page [API](https://developers.google.com/youtube/analytics/reference/reports/query?apix_params=%7B%22endDate%22%3A%222022-06-01%22%2C%22filters%22%3A%22video%3D%3DyVrdM-3f36w%22%2C%22ids%22%3A%22channel%3D%3DMINE%22%2C%22metrics%22%3A%22views%2CestimatedMinutesWatched%2CaverageViewDuration%22%2C%22startDate%22%3A%222021-06-01%22%7D&apix=true)

- Sample CURL call for single video with a date range.

```
curl \
  'https://youtubeanalytics.googleapis.com/v2/reports?endDate=2022-06-01&filters=video%3D%3DyVrdM-3f36w&ids=channel%3D%3DMINE&metrics=views%2CestimatedMinutesWatched%2CaverageViewDuration&startDate=2021-06-01&key=[YOUR_API_KEY]' \
  --header 'Authorization: Bearer [YOUR_ACCESS_TOKEN]' \
  --header 'Accept: application/json' \
  --compressed
```
- Get an API Key. Go to (Link)[https://console.cloud.google.com/apis/credentials?project=chips-youtube-apis-346416]

click create credentials

- To get the bearer token follow this (Link)[https://stevesie.com/docs/pages/youtube-oauth-access-token]
