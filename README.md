[**www.Instabus.org**](http://instabus.org)
====================

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/luqmaan/Instabus?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

#### [Realtime map of Austin's MetroRapid bus and MetroRail train](http://instabus.org)

[![](https://cloud.githubusercontent.com/assets/1275831/3210441/0128e4a2-eec1-11e3-8622-fc947f7c305c.png)](http://instabus.org)

##### Works on your desktop, your iPhone, and your Android device. Just go to [instabus.org](http://instabus.org)

![placeit](https://cloud.githubusercontent.com/assets/1275831/3565798/3078cb22-0ad3-11e4-8285-005d3c211766.jpg)


##### Watch the bus/train move in realtime on a map. Also see how fast (or slow) it is moving. This bus between Chinatown and Techridge is moving South at 39 mph.

![realtime-bus](https://cloud.githubusercontent.com/assets/1275831/3565764/29f44d6a-0ad0-11e4-9bc0-aa39e50b77a3.jpg)

##### See the next few arrivals at a glance.

![arrivals-at-a-glance](https://cloud.githubusercontent.com/assets/1275831/3565763/29f3796c-0ad0-11e4-9508-0b03d1fcd1b8.jpg)

## Routes

CapMetro provides realtime data for these routes:

- 801 North MetroRapid
- 801 South MetroRapid
- 550 North MetroRail
- 550 South MetroRail

## Problemo

- People don't ride the bus because it can seem unreliable: buses arrive anytime from 10 minutes before their scheduled time to 20 minutes after
- The solution to that is real-time data
- But if the real-time data is hard to access, people won't use it
- CapMetro's app has real-time data
- But, CapMetro's app is **hard** to use. See [CapMetroApp: When should I take the bus home?](https://github.com/sethgho/MetroRappidAndroid/wiki/CapMetro-App---When-should-I-take-the-bus-home)


## Solution

Step 1. Select A Route And Direction

![Select A Route And Direction](https://cloud.githubusercontent.com/assets/1275831/3613330/f7e6324a-0db6-11e4-96f9-77adfff913bc.png

Step 2. Instabus automatically finds the nearest stop and vehicle

![View the closest stop and vehicle](https://cloud.githubusercontent.com/assets/1275831/3613329/f7e0cdc8-0db6-11e4-972f-9de75b036372.png))

Step 3. Get on the bus. Let everybody around you know about [instabus.org](http://instabus.org)

## FAQ

### What happened to MetroRappid?

MetroRappid has been renamed to Instabus.

MetroRappid for iOS has been replaced with Instabus.

MetroRappid for Android (winner of ATX Hack For Change) had problems working with the Google Maps API. We've chosen to move in the direction of open data, and now instead use OpenStreetMaps. This webapp replaces MetroRappid for Android.

### Why don't I see any buses or trains?

We're relying on Yahoo! Query Language to provide a backend that allows us to talk to CapMetro's API (avoiding CORS issues). This is a hacky and unreliable solution. You should encourage CapMetro to make their API more easily accessible.

### Why is the vehicle location out of date?

CapMetro only updates the vehicle location every 30-90 seconds. You should encourage them to provide more accurate realtime data.

## Contributing

We really need help making this app awesome. We use GitHub issues to track bugs, features, and ideas. Issues that we think are important/can use help are tagged as `help wanted`. You can filter by the `help wanted` tag: https://github.com/luqmaan/Instabus/issues?labels=help+wanted&state=open.

Run `gulp deploy` when submitting a pull request. This packages up the .js and .css files.

### Installation

Clone the repo and checkout the `dev` branch:

```
git clone git@github.com:luqmaan/Instabus.git
cd Instabus
git checkout -b dev origin/dev
```

Install dependencies through [npm](https://www.npmjs.org/) and [browserify](http://browserify.org/):

```
npm install
```

Serve the directory with [gulp](http://gulpjs.com/):

```
gulp serve
```

### Deployment

To deploy:

```
gulp clean
gulp build
gulp deploy
```

## Contributors

- https://github.com/luqmaan
- https://github.com/drmaples
- https://github.com/paulserraino
- https://github.com/ECatx
- https://github.com/fleeting
- Mayhaps you?

## License

GNU General Public License Version 3
