
Kibo Manana
-------------

This is an android based app that is aimed at improving the connectivity as well as give suggestions in case of a disaster.

This app downloads the map of User's surroundings within a radius of 2 km from google maps for the offline use.

PRE DISASTER MODE:
--------------------

Goals:
------------------
To provide users with an idea of the impact that the disaster is going to have, going by the previous data and suggesting best possible solutions depending on various conditions like health of the individual,transport system of the place, connectivity etc.

Functionality:
--------------
The App is given root access and gets its prediction data from websites like UNISDR and Other Statistical Institutes across the Globe.

Once the prediction has been given by the Statistical Institutes about a disaster, this app starts running in the background.

Using Neural Network Algorithms it starts predicting the routes that would be damaged or the extent to which the damage might be caused, based on previous data regarding similar disasters at nearby locations and comes up with best possible routes that can be taken in case of a disaster using A* algorithm.

It also gives the probability of other disasters ensuing the current disaster,this would help people to understand how essential it is for them to evacuate the place prior to the disaster occurrence.

It also collects data of any medical condition that the user has and takes in account this factor to suggest action that has to be taken.

POST DISASTER MODE :
-----------------------

ASSUMPTION:
-----------------
High Population Density

Goals :
-------------
1.To help establish network among the users and help evacuation Teams track people in the affected area as Communication would be badly affected

2.To help navigate people to a nearby evacuation centre.

3.To connect and share supplies with people nearby.


Functionality:
--------------
The App must be put on the Post Disaster Mode by the user,it switches on the Hotspot and uses that to connect to other phones in the vicinity.

In other Words,One Phone acts as a Server.Every other phone that gets connected to this network, shares its connection through WiFi/Bluetooth Tethering.

Every mobile using the downloaded maps locates it position on the offline-map using GPS and broadcasts its coordinates on to the network.
All mobiles mark their coordinates in a text file which is circulated in the network.

Once a mobile with Internet connectivity is found in the network this data is sent to the Evacuation teams.
This helps rescue teams in locating people.

Users can locate and communicate with other users in their surroundings thus facilitating resource sharing
It also helps them to gather in groups which would make their rescue simpler.


Stage 3 :
--------------------
Goal:
------------------
To Save the Battery of the Mobile,Using zero configuration networking the mobile that acts as the server keeps changing.

For an instance,if mobile-1 is initially acting as the server,in case of low battery,mobile-2 becomes the server as it would be battery draining to act as the server.
