# leaflet-map-image-overlay
An interm attempt at adding support for the imageOverlay layer type to the [leaflet-map](https://github.com/leaflet-extras/leaflet-map/) project.

The goal is to allow for using the Leaflet webcomponent as a UI for large images following the example in the [Using leaflet.js to pan and zoom a big image](http://kempe.net/blog/2014/06/14/leaflet-pan-zoom-image.html) blog post.

Hopefully this project will be merged or superceded by the result of this github issue: https://github.com/leaflet-extras/leaflet-map/issues/82

If syncing from git directly, run the examples by creating a .bowerrc file as described here: https://divshot.com/blog/web-components/polymer-and-bower-getting-it-right/
Not included by default to prevent accidently polluting file system

Known issues:
The original blog post describes changing the crs value of the map object to L.CRS.Simple. It looks like that change would require a modification to leaflet-core to expose that property when creating the underlying map. I'm not sure if this is necessary or the implications of not adjusting the crs value.
