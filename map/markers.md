## Map Markers

1. The script.js file is setup so it is easy to edit. 

Example of a marker code:

    			{
      				type: "Feature",
      				geometry: {
        				type: "Point",
        				coordinates: [-76.469368, 44.77903]
      			},
     				properties: {
        				title: " Camp Opemikon",
        				description:
          				'<a href="https://community.scouti.tk/topic/opemikon">Community topic</a>'
      			}
    				},
 
**YOU NEED TO HAVE A MAPBOX  ACCSES TOKEN! LEARN MORE AT: [https://scouti.tk/maptokens](https://scouti.tk/maptokens)**



Change your third line on script.js file to look like this!

				mapboxgl.accessToken =
  				// Your token goes here. This will not work on your site. se more at https://scouti.tk/maptokens
  				"##.YOUR TOKEN HERE!!!!";
