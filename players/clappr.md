# Clappr video player integration

Add the following script on your HTML:

```html
<head>
  <!-- Clappr video player -->
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/clappr@latest/dist/clappr.min.js"></script>

  <!-- Kinow Video Analytics for Clappr -->
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/kinow-video-analytics@latest/dist/clappr.min.js"></script>

  <div id="player"></div>
</head>
```

```javascript
// Setup your video player like that:
let clappr = new Clappr.Player({
});

// Kinow Video Player Analytics
let videoAnalytics = new VideoAnalytics.Clappr({
  player: clappr, // Your Clappr video player
  hostingId: <integer>,
  videoId: <integer>,
  customerId: <integer>,
  datas: {
    isoCode: "<string>" // Iso code for your customer country
  },
});
```
