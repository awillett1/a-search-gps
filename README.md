# a-search-gps
An A*Search GPS implementation using Python for my final project in my Artificial Intelligence course.

**Implementation**
I created different classes for Cities, Roads, and Maps.
I included functions for adding cities and roads. I decided to use the Haversine Distance formula as my heuristic because it calculates the latitude and longitude between two points to find the shortest distance. My A*Search used the distance of each road as its cost formula.

I imported City and Road name information from https://github.com/thekaranacharya/road-trip-planner. I added the Roads and Cities to a database. I then added all of these to a Map.

I decided to test my A*Search with smaller subgraphs (Map with just the two Cities and one in-between.), like the optimal route between Bowdon, North Dakota and Franklin, Tennessee.

Later, I decided to change the A*Search cost to be time instead of distance (based on speed limits of the road): `(road.distance / road.speed)`

I also created a version of A*Search that avoided roads that had a speed limit over 50mph (assuming 50mph+ means it is a highway.)
