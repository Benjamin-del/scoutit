---
redirect_from: /
published: true
---

## ScoutIT campmaps.

This article refers to the creation of personal scoutIT map clones. 

ScoutIT camp maps is an open-sorce project. You can create your own version of the map! 


## Requirments 
1. A Github **OR** Glitch Account.
2. A Mapbox accses token. [https://scouti.tk/maptokens](https://scouti.tk/maptokens)
3. A Computer

## Cloning Code

1. Fork the repo. You need to make a copy of the repo. go to [https://github.com/Benjamin-del/campmaps](https://github.com/Benjamin-del/campmaps) to fork it.
	a. You can also use glitch ([https://glitch.com/help/kb/article/20-can-i-import-code-from-a-github-	repository/](https://glitch.com/help/kb/article/20-can-i-import-code-from-a-github-repository/)

2. Enable github pages. Go into the settings and select github pages. If you are using glitch your project this step is already done!

3. You are done! You can now add and change positions in of markers!

I find glitch is easier for beginners to understand. Github Has more features though.

## Adding your token (Required)

Change your third line on script.js file to look like this!

				mapboxgl.accessToken =
  				// Your token goes here. This will not work on your site. se more at https://scouti.tk/maptokens
  				"##.YOUR TOKEN HERE!!!!";

## Edditing markers

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

## Images.
To change the map markers replace marker.png in /images to your image
To change the favicon replace favicon.ico with your image.

## Map styles
line 7 = Map Style
line 8 = Onload center
line 9 = Onload zoom 

   Example: I used the satilite style:

	var map = new mapboxgl.Map({
  	container: "map",
  	style: "mapbox://styles/mapbox/satellite-v9",
  	center: [-76.469368, 44.77903],
  	zoom: 6
	});

List of styles: [https://docs.mapbox.com/api/maps/styles/#mapbox-styles](https://docs.mapbox.com/api/maps/styles/#mapbox-styles)

## Public views 
(Index.html / home.html)

ScoutIT campmaps comes with all of the required images. I ask that you change favicon.ico file. The markers you can keep.

Index.html
This page is not in use. It will redirect to home.html.

Home.html 
This page can be edited and changed. If you dont want it un-comment line 8

 				<!--<meta http-equiv="refresh" content="0;url=map" /> -->
 TO

 				<meta http-equiv="refresh" content="0;url=map"/>


 Beta.html.
 This page is not edditable (I Used a different application to build it) You can just delete it.
 If you do delete it comment/remove line 25 in home.html





