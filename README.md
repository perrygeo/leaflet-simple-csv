Simple Leaflet map template for putting points on a map.

<img src="https://raw.github.com/perrygeo/leaflet-simple-csv/master/img/screenshot1.png" alt="Leaflet" />

### Features
* Data is in tabular delimited-text (csv, etc.) with two required columns: `lat` and `lng`
* Points are plotted on full-screen [Leaflet](https://github.com/Leaflet/Leaflet) map
* Point markers are clustered dynamically based on zoom level.
* Clicking on a point cluster will zoom into the extent of the underlying features.
* Hovering on the point will display the name. 
* Clicking will display a popup with columns/properties displayed as an html table.
* Full text filtering with typeahead
* Completely client-side javascript with all dependencies included or linked via CDN

###
### Usage
Download, copy the template and load index.html in a browser to confirm that everything works

```
git clone https://github.com/perrygeo/leaflet-simple-csv.git
cd leaflet-simple-csv
cp config.js.template config.js
open index.html
```

Then modify `config.js` and `data/data.csv` according to your needs.

Some browsers do not allow XMLHttpRequests with the `file://` protocol so you'll need to serve it with a web server. For local development, you can use python

```
$ python -m SimpleHTTPServer
Serving HTTP on 0.0.0.0 port 8000 ...
```
Then navigate to `http://localhost:8000` instead.

### Thanks to...

* [Leaflet](https://github.com/Leaflet/Leaflet)
* [Leaflet.geoCSV](https://github.com/joker-x/Leaflet.geoCSV)
* [Leaflet.markercluster](https://github.com/Leaflet/Leaflet.markercluster)
* [Twitter Boostrap](http://twitter.github.io/bootstrap/)
* [jQuery](http://jquery.com/)

