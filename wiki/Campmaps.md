## ScoutIT campmaps.

This article refers to the creation of personal scoutIT map clones. 


## Requirments 
1. A github OR glitch account.
2. A Mapbox accses token. [https://scouti.tk/maptokens](https://scouti.tk/maptokens)
3. Computer

ScoutIT camp maps is an open-sorce project. You can create your own version of the map! 

1. Fork the repo. You need to make a copy of the repo. go to [https://github.com/Benjamin-del/campmaps](https://github.com/Benjamin-del/campmaps) to fork it.
	a. You can also use glitch ([https://glitch.com/help/kb/article/20-can-i-import-code-from-a-github-	repository/](https://glitch.com/help/kb/article/20-can-i-import-code-from-a-github-repository/)

2. Enable github pages. Go into the settings and select github pages. If you are using glitch your project this step is already done!

3. You are done! You can now add and change positions in of markers!

I find glitch is easier for beginners to understand. Github Has more features though.


## Adding markers

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

## Adding your token (Required)

Change your third line on script.js file to look like this!

				mapboxgl.accessToken =
  				// Your token goes here. This will not work on your site. se more at https://scouti.tk/maptokens
  				"##.YOUR TOKEN HERE!!!!";
