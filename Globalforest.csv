const map = new mapboxgl.Map({
  container: 'map',
  style: 'https://api.mapbox.com/styles/v1/mapbox/satellite-streets-v11',
  center: [0, 20], // Center of the world
  zoom: 2
});

// Add forest loss layer
map.on('load', function() {
  map.addLayer({
    'id': 'tree_loss',
    'type': 'fill',
    'source': {
      'type': 'vector',
      'url': 'mapbox://globalforestwatch.treecoverloss'
    },
    'source-layer': 'tree_cover_loss',
    'paint': {
      'fill-color': '#ff0000',
      'fill-opacity': 0.6
    }
  });
});
