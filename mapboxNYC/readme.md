# Mapbox+Unity SDK

## Part One - Mapbox + Unity - Installation

Download the unity package from https://www.mapbox.com/install/unity/

In Unity, go to Assets > Import Package > Custom Package
This adds a Mapbox option in the menu bar of Unity

Go to Mapbox > Setup > paste your mapbox access token 

Go to the examples folder in Mapbox and run an example.. It should work! 

## Part Two - Mapbox + Unity - 3D Buildings

The create > Mapbox option has 5 options 
- Modifiers
- MapVisualizer 
- Factories
- Filters
- Layer Visualizer 

The map editor shows a nice flow chart of what's connected to what - This is important cause there's a lot of layering happening here. 

First Layer you need is the 
BasicMapVisualizer

The second layer is the Terrain mesh layer 
This is inside of Factories > Terrain Factory

This Terrain needs to connected in the BasicMapVisualizer's inspector under factories

You can also set a loading texture so it says LOADING when it is yet to load the tiles
You can use Height Multiplier to exaggerate the heights of buildings

The third layer is the ImageFactory
Mapbox > Factories > Image Factory

Add an empty Gameobject named Map and add the component Basic Map - set Map Visualizer to CityMap

Set Latitude/Longitude based on what you want the location to be - Zoom in 16 or more

Add Range Tile Provider component to Gameobject Map - set Range 1,1,1,1

The fourth Layer is VectorTileFactory 
This is also in Mapbox > Factories > Vector Tile Factory

Add this vectory tile factory to Map visualizer









