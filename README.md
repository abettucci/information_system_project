# information_system_project

As a product of this project, there are currently Internet access points on the WIFI network.
of País Digital which provides free internet access in public spaces and facilities throughout the country.
The system to be implemented will consist of a program that analyzes the information of the points that they provide
free internet access in public spaces and facilities throughout the country and manage the
connections and disconnections of users to them.

The data is real and obtained from the corresponding page of the National Government.
Two example files are attached to the statement: 
- The first, “municipios.csv”, contains the definition
of a set of municipalities, in their respective departments, in turn within their respective
provinces
- The second contains information on the access points available in each municipality.

Both the front and back end were developed in Python.
The front end was made with PyQt library and the design was facilitated with Qt designer for the windows design of the system.

Considerations:
- An access point can be installed or broken at any time.
- When a user inputs invalid data, a notification is shown to make the corresponding changes.
- Computers are identified with a unique MAC address of the equipment in the world, and at the same time
to connect, the access point must assign you a unique IP address on that router (i.e. you can
there may be repeated addresses on different routers). For simplicity, both IPs and
MACs were considered as integers, although this is not the case in the real world.
- An access point can have a maximum of 20 simultaneous connections.
- It should be noted that the IDs of the secondary locations (municipalities and departments) are only unique
within his supraadministration. That is, there can be two municipalities with the same id, while
are in different departments, in the same way that two departments can exist
different as long as they are in different provinces.

System must be able to:
- The system must be able to manage different access points (access point, or, colloquially,
WiFi antennas) distributed throughout the national territory. Access points must be added or
removed from the system when they start or stop working in the real world.
- The system must in turn allow users' computers to connect or disconnect from a access point. The computer should only be able to be connected to a single access point to the time.
- The system must be able to print the number of active connections (not closed) in a province,
given municipality or department. That is, I can ask for the number of active connections (not closed)
currently from the entire Province of Buenos Aires, or from the municipality of 9 de Julio only.
- The system must allow viewing all connections in the national network in a
certain time interval (for example, all connections that were started between yesterday and
2 in the afternoon and today at 4:05 in the morning). This goes for all connections, whether they are still
open or closed.
- The system must be able to persist its information between system closures. That is, all the information
in the system, after closing, should still be there when you reopen the program, without the need to
perform any manual procedures as a user. The only way to shut down the system will be through the corresponding menu option.
