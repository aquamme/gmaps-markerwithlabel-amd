gmaps-markerwithlabel-amd
=========
Based on [Google Maps MarkerWithLabel 1.1.9](http://google-maps-utility-library-v3.googlecode.com/svn/tags/markerwithlabel/1.1.9/).
This is basically a fork of the fork that adds src/markerwithlabel-amd.js.

This extension offers AMD support for Google Maps MarkerWithLabel utility library of Google Maps Javascript API v3. Also fixes the problem with requirejs optimizer. Also fixes the label overlap issue with the fix given in comment #28 [here](https://code.google.com/p/google-maps-utility-library-v3/issues/detail?id=24&colspec=ID%20Type%20Status%20Priority%20Fixed%20Owner%20Summary%20Stars).
Dependencies
----
[requirejs async plugin](https://github.com/millermedeiros/requirejs-plugins/)
Install
----
```
bower install google-markerwithlabel-labelfix
```

```
git clone https://github.com/aquamme/gmaps-markerwithlabel-amd
```
Usage
----
```
paths: {
    require.config({
        /* Bower Libraries */
        async: '../bower_components/requirejs-plugins/src/async',
        markerlabel: '../bower_components/google-makerwithlabel/src/markerwithlabel-amd',
...
```

```
var MarkerLabel = require('markerlabel');
...
var myMarker = new MarkerLabel({ ... })
```
License
----
Apache 2.0
