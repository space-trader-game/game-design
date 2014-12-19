# Game Components
Every game has various components. Here is a general overview of some of the
components and functions and etc.

## Main Menu
* Configuration options
* New game
* Load Game

## Maps 
### Generator
When a new game is started, either pre-defined maps will be selected, or a
random map can be generated. The map generator component will be what handles
creation of random maps. It will need to take some input options (for example,
map size, system density, etc) and use those to generate a map.

### Map and Data
The game will feature hex-based maps. A data structure needs to be determined
for storing map data. The map data only contains:

* Systems
  * Their locations
  * Information about them (slots, etc)
* Galaxies
  * The borders of galaxies

### Hex Grid Information
[Red Blob Games - Hexagonal Grids](http://www.redblobgames.com/grids/hexagons/)

## Current Game Data
A data structure is needed to store data about the current game state including:

* what is on the map where (eg: ships and other objects)
* current state of players
  * money
  * whose ships are whose
  * etc
