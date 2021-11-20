<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>Display a map on a webpage</title>
<meta name="viewport" content="initial-scale=1,maximum-scale=1,user-scalable=no">
<link href="https://api.mapbox.com/mapbox-gl-js/v2.6.0/mapbox-gl.css" rel="stylesheet">
<script src="https://api.mapbox.com/mapbox-gl-js/v2.6.0/mapbox-gl.js"></script>
<style>
body { margin: 0; padding: 0; }
#map { position: absolute; top: 0; bottom: 0; width: 100%; }
</style>
</head>
<body>
<div id="map"></div>
<script>
	mapboxgl.accessToken = 'pk.eyJ1IjoibWF0ZWpld3MiLCJhIjoiY2t3Mml4M3hiYWN2dzMwcXAxZm9vajFnOSJ9.iEsyjKbZpd4iujEGtfN5bQ';
    const map = new mapboxgl.Map({
        container: 'map', // container ID
        style: 'mapbox://styles/matejews/ckw2j1tgs28wy14s9oa29amrh', // style URL
        center: [-78.024902, 37.926868], // starting position [lng, lat] //I have moved the - sign from this vs. 11-19
        zoom: 11 // starting zoom
    });
</script>

</body>
</html>
