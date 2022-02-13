# Mapping_Earthquakes
## module 13 challenge

I enjoyed this challenge.  It's fun playing with the maps.  It's also cool to know that the data we used is current, and not out of date.
There were 3 parts to this challenge:
1. adding the tectonic plates lines to the map
2. creating a layer for just the major earthquakes
3. adding a third base option (dark) to the streets and satellite options for the map

The third part was pretty easy, so I did that first.  My maps had 3 options for the base layer the whole time I working on it.
I had a little trouble accessing the data for the tectonic plates and was getting CORS errors.  I was able to resolve it by downloading the data file instead of accessing it directly on the web.  I also played with using different colors for the tectonic plate lines.  I think yellow shows up the best on the different maps.
The layer for just the major earthquakes was very similar to the layer with all of the earthquakes, just needed a little tweaking of the code.

## Things I changed about the maps
1. I shifted the center of the map, so it initially shows more of the whole world.  The original Latitude and Longitude coordinates were inside America and didn't show the far east, where many of the earthquakes are located.  
2. I changed the colors for the major earthquakes to try to emphasize the difference in magnitude.  The colors do not exactly match the colors that are on the "all earthquakes" map.
3. I also changed the formula for the diameter of the circles on the major earthquakes map.  Earthquake magnitude is a logarithmic function, so just multiplying by a base number doesn't do a good job of showing the difference between larger earthquakes.  I squared the magnitude - which still isn't a logarithmic function but it does better show the size difference.

## Things I want to change
1. I don't like how the legend at the bottom of the map doesn't change depending upon which layer you choose to look at.  The legend applies to the "all earthquakes" layer, but it doesn't apply to the major earthquakes layer or the tectonic plate layer.  I wish the legend would be attached to (and could change for) each layer, instead of being applied on top of them.
