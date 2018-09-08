# GovHack2018Expose
Expose's Gov Hack 2018 project

** Challenges: **
- Local - Improving Response - Best entry that assists CFS planning for and responding to incidents
- National - Working Together - How can open government data to improve responsers' situational understanding and ability to plan their response, and share their information between agencies? How can sharing information between agencies be improved by different information presentation, allowing more informed decisions during domestic emergencies or national security events?

#### Data Collection and Identification:
What data could we find that was open for use within the GovHack 2018 competition. As a team we worked together to identify all the open licensed data sets, and Data Services we could freely use and repurpose to meet the above challenges. Immediately we interepreted the challenges as needing mapping data sets; location based, as well as other real time data feeds. There's the data needed for preparation for those ready to confront whatever incident or emergency is occuring, there's the data needed to collect information about the incident, as well as peripheral data such as weather, rainfall\wind direction that is currently occuring. There's also the data to assist the services to reach the incident efficiently and safely, as well as those near the incidents to move away from danger as quickly and safely as possible. Once the relevant services are within proximiatey of the incident or emergency, they need continuous feeds of data to locate those injured or in danger, knowing where the exact front of the fire or emergency is, what risks are a factor, but also relying on constant communication to other emergency services, planes, applicances, volunteers and control centres. Basically, we wanted to find any data sets that may have been useful for any of these purposes.    

#### Using the data, merging together and making available for users and contributors
With complex and different types of data sets, a necessary step is to land this data onto a shared platform, either using a traditional relation database platform, or more modern data stores like cosmos db which can handle semi structured data, to even something less complicated such as BLOB storage. Regardless of the platform, data can then be fed into a number of services using a real time messaging, or streaming service to push data out using a broker which can then be subscribed to by which ever agencies need it. The same source of data can be used by a number of agencies at the exact same time seeing the same data but potentially in a different format. i.e. A member of a CFS applicance may only want to know details of members of the same applicance, where as their regional chief, needs to know data about several appliances, and a control centre may need to know everything but in summary. All same data, all being pushed out at once, and can be used in different ways by different subscribers. Can also be used by Apps or reporting tools, but being stored in a database gains access to more complex processes like machine learning over historical data. The app can also play the role of data contributor too, allowing users to enhance the data further by inputting more accurate and real time substance such as if a fire or threat has moved, so that everyone can subscribe to that information.  

#### Going further than that!
There is plethora of data that 'could' be collected to further enhance the challenge to plan and repsond to emeregencies even better. Having each vehicle, applicance, plane or helicopter to name a few, tracked by a device to publish to all involved where a vehicle is at at any point in time, their fuel load and/or their water load (if water bomber or fire appliance). This could extend to individuals on the ground tracking where each servicemen is located, for a variety of benefits from a rescueing point of view, but proximatey to the closest threat or person in need. More compicated devices could be used to locate people in distress either using meshing technology to locate a phone signal, or provide them with beacons so they can be located, with the beacons also sending data to the platform which can be used throughout the solution. Therefore, each entity within the environment of concern can be located and tracked, therefore more complex alogirthms can be sued in combination of this data to find the best possible method of extracting those from danger, whilst focusing on retarding the threat. If a threat is a person or people, this too can be identified using facial recognition, and tracked and pin pointed using a variety of Artificial Intelligence API's. 

Team memebers: Etienne Oosthuyesen, Jean-Noel Seneque, Jake Deed, Andrew Exley and Cameron Wells

Source Code url: https://github.com/ExposeShowUsYourData/GovHack2018Expose

Video url: 

Homepage url: https://github.com/ExposeShowUsYourData/GovHack2018Expose

### Local Event Location:

Adelaide

### Datasets Used:

* Aquatic Ecosystem Condition Reports - Environment Protection Authority (EPA) - South Australia
https://data.sa.gov.au/data/dataset/aquatic-ecosystem-condition-reports The aquatic ecosystems condition data provides details on water quality, aquatic habitats and protected sites which provides the locations of specific species for our platform. The data also provides information on water quality on the sites featured on our app.

* Shorebased Recreational Fishing - Dept of Environment, Water and Natural Resources
https://data.sa.gov.au/data/dataset/shore-based-recreational-fishing The recreational fishing related locations will be used to guide users of Aquadex app. The spatial data will be used for map display as well as augmented reality interfaces.

* Jetties - DPTI
https://data.sa.gov.au/data/dataset/jetties/resource/b617df1e-345b-47e4-a61e-445487a2be9f The spatial data is used to visualize locations of related activities in our app using interactive maps and augmented reality interface.

* South Australian Boat Ramp Locator - DPTI http://data.gov.au/dataset/05546e03-2997-4762-a439-0f2e9a492650 The spatial data is used to visualize locations of related activities in our app using interactive maps and augmented reality interface.

* Whale Sightings Log - SA Whale Centre
http://www.sawhalecentre.com/whale-sightings/sightings-log/?mc_cid=00ccaf0043&mc_eid=3b8b4f019a Current and past whale sightings logs will be used used to extract location data and descriptions to be displayed through aquadex app.

* South Australian Shipwrecks Database https://data.sa.gov.au/data/dataset/shipwrecks The spatial data is used to visualize locations of past shipwrecks using interactive maps and augmented reality interface.

### APIs Used

* Awe.js: Used to simplify using HTML5 geolocation, orientation and WebGL

* Three.js: Used as a cool WebGL library

* Google Maps JS API: Used to superimpose a layer of Roads and Streets with names on top of the camera feed.

* Google Maps Directions API: Used for routing and navigation from user's current location to destination (location of restaurant, club, etc.)

* Backendless: On-demand Mobile Backend as a Service (mBaaS) platform.

* Monocular API (not used in the PoC): Can be used to identify species. 
