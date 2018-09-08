![Expose:Show us your data logo](expose_Logo_Colour_transparent.png)

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

* Dams (Angus Catchment) - Department for Environment and Water - South Australia
https://data.sa.gov.au/data/dataset/dams-angus-catchment The Angas Catchment Dams dataset is a subset of the Hydro Water Bodies dataset and is limited geographically to the Angas River surface water catchment in South Australia. The data set contains polygon data outlining the physical extent of dams and estimated dam capacity (volume range in megalitres) and wall height information (in metres). Dam capacities have been estimated using various methods. These capacities have been converted to volume ranges. The majority of wall heights have been measured on site using a hand sight level. Dam capacity and wall height is based on available information and although best effort and care has been taken in compiling this information, accuracy cannot be guaranteed. The dataset will change over time as further information becomes available. 
The data is used to identify where water resources are located and quantity of water (estimated).

* PSMA Geocoded National Address File (G-NAF) - Department of Industry, Innovation and Science
https://data.gov.au/dataset/19432f89-dc3a-4ef3-b943-5326ef1dbecc/gmd G-NAF is one of the most ubiquitous and powerful spatial datasets. It contains more than 13 million Australian physical address records. The records include geocodes. These are latitude and longitude map coordinates. G-NAF does not contain any names or personal information.
Data is used for multipile locations of interest, from petrol stations, police stations through to schools and hospitals.  

* Contours - Geoscience Australia
http://services.ga.gov.au/gis/rest/services/NM_Relief_and_Physiography/MapServer Esri ArcGIS MapSever URL. The web map service portrays detailed graphic representation of features that appear on the Earth's surface. These features include the relief and physiography themes from the Geoscience Australia 250K Topographic Data.
Data is used to associate gradiant with landscape. This is important in predicting where water will flow next, where fire may increae in intsity, but also for people or vehicles to cross terrain. 

* Last Bushfire and Prescribed Burn Boundaries - Department for Environment and Water  - South Australia
http://www.waterconnect.sa.gov.au/Content/Downloads/DEWNR/FIREMGT_LastFire_shp.zip The dataset provides most recent fire scar mapping for many major fires that have burnt in a given area within or adjacent to National Parks and Wildlife South Australia (NPWSA) reserves. This data set is derived from Fire History mapping. The most recent fire mapping can be used for operational management and planning of fire events and ecological resource management.
Used to indicate risk of fire fuelling up due to no recent fires through the location. Can help predict intensity of fire which can indicate if an evacuation route is safe or not. 

* Airport Point Features - Geoscience Australia
http://services.ga.gov.au/gis/rest/services/NM_Transport_Infrastructure/MapServer Esri ArcGIS MapSever URL. This Airports (Point features) layer complements the Airport Runway Centrelines and Landing Grounds (Line features) Layer in this web mapping service. 250K Specification Description - Airport Area - The defined area of a facility licensed, certified or registered by the Civil Aviation Safety Authority intended to be used either wholly or in part for the arrival, departure and surface movement of aircraft and associated cargo. Runway Centreline - A line used to indicate the length and orientation of an airport's runway.
Used to locate airport infrastructure which is used to indicate where water bombers may land to refill or evacute in an emergency.

* Recent Air Quality - Environment Protection Authority (EPA) - South Australia
http://www.epa.sa.gov.au/air_quality/pi.txt RSS feed. TThe EPA’s recent air quality data is a RSS feed that includes hourly average pollutant concentrations for ozone (ppm), carbon monoxide (ppm), nitrogen dioxide (ppm), sulfur dioxide (ppm), particles (PM10) (μg/m3), fine particles (PM2.5) (μg/m3) and station index (station air quality index or AQI) for 13 EPA monitoring sites.
Used to locate airport infrastructure which is used to indicate where water bombers may land to refill or evacute in an emergency.
Used for in national disaster or tracking potential threats to nation. RSS feed updated hourly can track if any toxic chemicals detected in different areas. Have thresh holds for safe ranges but in the event of Chemical bomb, Nuclear particles etc can detect if there is any change in air monitoring and pin point where issues or unsafe areas are.

* Real Time Traffic Delays - Department of Planning, Transport and Infrastructure - South Australia
http://maps.sa.gov.au/AddInsight/geoservice/links This web service provides details of traffic delays that are currently active in the metropolitan Adelaide area updated every 30 seconds
In an emergency congestion can be critical to avoid for an immediate emergency response vehicle attending an emergency

* Road Bridges and Fords - Geoscience Australia
http://services.ga.gov.au/gis/rest/services/NM_Transport_Infrastructure/MapServer Esri ArcGIS MapSever URL. Road Bridge Point - A structure erected over a depression or obstacle to carry road traffic. Ford Point - A shallow or flat portion of the bed of a watercourse or lake where a crossing may be affected.
Locations to protect, but also use when necessary to transport cars\trucks to or from danger

* Roads - Department of Planning, Transport and Infrastructure - South Australia
http://www.dptiapps.com.au/dataportal/Roads_shp.zip Roads - A structure erected over a depression or obstacle to carry road traffic. Ford Point - A shallow or flat portion of the bed of a watercourse or lake where a crossing may be affected.
Locate all public sealed\unsealed roads as well as private roads

* Mobile Black Spot Database - Department of Communications and the Arts
https://data.gov.au/dataset/7be6e3ee-043a-4c47-a6eb-a97702419ccd/resource/c6b211ad-3aa2-4f53-8427-01b52a6433a7/download/mbsp-database-of-reported-locations-2016-electorates.csv - The Department of Communications and the Arts has received nominations of regional locations with poor or no mobile coverage from members of the public. The database was used by applicants to design their proposals for funding under round 1 of the Mobile Black Spot Programme and is again being used for round 2 of the programme.
Cruicial information when communications is necessary. Can be used to bring in additional temporary infrastructure to handle communications for communities during an emergency if included as a data set.  

* Water Supply Reserves - Geoscience Australia
http://services.ga.gov.au/gis/rest/services/NM_Reserves/MapServer - Water Supply Reserve - Land reserved to protect water supply catchments.
Water Supply Areas to protect from contamination or use to retard fire.

* Homesteads - Geoscience Australia
services.ga.gov.au/gis/rest/services/NM_Labelling_and_Boundaries/MapServer - Residential Buildings - A permanent walled and roofed construction or the ruin of such a construction. Residential Buildings are used principally as dwellings
Use to identify where homesteads are so to identify how to remove people from homesteads, away from danger and the danger's potential paths, but also where peoples homes are so to protect

* Statistical Area Level 1 (SA1) - ABS 
http://www.abs.gov.au/ausstats/subscriber.nsf/log?openagent&1270055001_sa1_2011_aust_shape.zip&1270.0.55.001&Data%20Cubes&24A18E7B88E716BDCA257801000D0AF1&0&July%202011&23.12.2010&Latest
Boundries of SA1 areas could be used in combination with incidents and statistical population to estimate people affected or likely to be affected by incident. People likely to need to be evacuated etc.

* Storage Tanks - ABS
http://services.ga.gov.au/gis/rest/services/NM_Culture_and_Infrastructure/MapServer This service has been created specifically for display in the National Map and the chosen symbology may not suit other mapping applications. The Australian Topographic web map service is seamless national dataset coverage for the whole of Australia. These data are best suited to graphical applications. These data may vary greatly in quality depending on the method of capture and digitising specifications in place at the time of capture. The web map service portrays detailed graphic representation of features that appear on the Earth's surface. These features include culture, habitation, industry and utility themes from the Geoscience Australia
Either prevent danger from reaching these key locations, or use them for leverage to assist with an emergency response

