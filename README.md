# Code_FunDo-
README
-------
NAME OF THE APPLICATION : Kibo Manana(Tentative)

It is an android based application that is aimed at improving the connectivity as well as give suggestions in case of a disaster.


THE PHILOSOPHY OF THE APP:
--------------------------
Natural disasters would be nothing but a series of events if not for human and monetary losses.
so, if we can avoid loss of human life then we would, in a sense be able to avoid turning a natural event into a natural disaster and hence, preventing a disaster from happening.

FUNCTIONALITY OF THE APP
------------------------------
WHAT DOES THE APP COME WITH WHEN INSTALLED
------------------------------------------
The app downloads your current location and the map of its surroundings within a radius of 2 km from google maps for the offline use.

It's functionality can be divided into 2 stages:
1. Pre  disaster stage
2. Post disaster stage


THE PRE DISASTER STAGE:
----------------------

Goal of this stage:
------------------
To provide users with an idea of the impact that the disaster is going to have, going by the previous data and suggesting best possible solutions (like would it be better if that individual relocates before disaster hits) depending on various conditions like health of the individual,transport system of the place, connectivity etc.

Functionality:
--------------
The App is given root access and gets its prediction data from websites like UNISDR(United Nations Office for Disaster Risk Reduction) and Other Statistical Institutes across the Globe.
Once the prediction has been given by the statistical Institutes about some disaster, this app starts running in the background and this mode is be called Pre disaster mode.

It starts predicting the routes that would be damaged or the extent to which the damage might be caused, based on previous data regarding similar disasters at the user's location and come up with best possible routes that can be taken in case of a disaster using A* algorithm.
It also gives the probability of other disasters ensuing the current disaster.

For Example:
If there is a nuclear plant near the seashore, what is the probability of a nuclear disaster happening depending on the Scale of the earthquake or Tsunami.(The Fukushima Incident,2011).

This probability would help people to understand how essential it is for them to evacuate the place prior to the disaster Occurence.
It also Collects data of any Medical Condition that the user has and takes in account this factor to suggest if it would be better if the user starts relocating now or can he stay at the site where disaster has been predicted to occur.

Technologies that We Might be Using to Realise these Functionalities:
----------------------------------------------------------------------
1.Neural network algorithms to predict possible damage to the navigation system or the resources using the data on previously occurred disasters at that place.

2.A-star algorithms to get best routes to be taken and possible steps to be taken using data that we got from neural network algorithms.

Note:
-----
The Reason Behind taking Predictions from UNISDR and other Statistical Institutes and not predicting them on our own is because of the accuracy of predicted data and the complexities involved in their prediction.


THE POST DISASTER MODE :
-----------------------
Assumptions:
------------
1.Connectivity has been partially/completely damaged.

2.High population density at the area.

Goals of this stage:
-------------------
1.To help establish network among the users and help Disaster Management Teams track people in the affected area.

2.To help navigate people to a nearby Evacuation Centre.

3.To connect and share supplies with people nearby.

Functionality:
--------------
The App must be put on the Post Disaster Mode by the user.
Then the App switches on the Hotspot and using that Connects to other phones in the vicinity.

There are Two Proposed Ways to Establish a Network Among Users:
-----------------------------------------------------------------
1.Using Bluetooth Tethering.

2.Using a Mobile Acting as a Wifi Repeater/Wifi Tethering.

In other Words,One Phone acts as a Server.Every other phone that gets connected to this network, shares it's connection through WiFi Tethering (By Acting as a Wifi Repeater) or through Bluetooth Tethering.This connection is continued until there is a mobile in the network that has internet connectivity to it.

Every mobile using the downloaded maps locates it position on the offline-map using GPS and broadcasts it's coordinates on to the network.
All mobiles mark their coordinates in a text file and the text file is circulated in the network.

Once a mobile with Internet connectivity is found in the network this data is sent to the Evacuation teams.

If a user gets disconnected from the network, he/she can approach a nearby user or this app gives last known location of the missing person.
This helps rescue teams in locating people almost accurately.

In meantime, the users can locate other users in their surroundings using their coordinates and can also inform others regarding any blockage in the path they are taking and hence circulating information.Hence a communication is established between people nearby which facilitates resource sharing and helps them to gather in groups which would make it easy for the evacuation teams to locate and rescue them.

Stage 3 : (Optional)
--------------------
Goal of the Stage:
------------------
To Save the Battery of the Mobile,Using zero configuration networking the mobile that switches on the hotspot (The Server) keeps changing depending on the battery level.
For an instance,if mobile-1 is initially acting as the server for the network ,in case of low battery,mobile-2 becomes the server for the network as being a server (i.e,switching an hotspot) would be battery draining.
