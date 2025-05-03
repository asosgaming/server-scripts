# server-scripts
Scripts for server management

## Firewall Functions
This section contains functions to manage the firewall on a server. The functions allow you to check the status of the firewall, manage firewall zones, and handle ports, protocols, and services associated with those zones.

|Name|Description|
| --- | --- |
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Active}$|Check if the firewall is active.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Inactive}$|Check if the firewall is inactive.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}$|Check if a specific firewall zone exists.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Delete}$|Delete a specific firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Create}$|Create a new firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Source}$|Check if a source is associated with a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Source}{\color{white}:}{\color{magenta}Add}$|Add a source to a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Source}{\color{white}:}{\color{magenta}Delete}$|Delete a source from a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Interface}$|Check if an interface is associated with a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Interfaces}$|Get all interfaces associated with a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Interface}{\color{white}:}{\color{magenta}Add}$|Add an interface to a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Interface}{\color{white}:}{\color{magenta}Delete}$|Delete an interface from a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Target}$|Set or get the target of a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Port}{\color{white}:}{\color{magenta}Add}$|Add a port to a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Port}{\color{white}:}{\color{magenta}Delete}$|Delete a port from a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Ports}$|Get all ports associated with a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Protocols}$|List all protocols associated with a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Protocol}{\color{white}:}{\color{magenta}Add}$|Add a protocol to a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Protocol}{\color{white}:}{\color{magenta}Delete}$|Delete a protocol from a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Services}$|Get all services associated with a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Service}{\color{white}:}{\color{magenta}Add}$|Add a service to a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Service}{\color{white}:}{\color{magenta}Delete}$|Delete a service from a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zone}{\color{white}:}{\color{magenta}Service}$|Check if a specific service exists in a firewall zone.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zones}$|Get all firewall zones.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Zones}{\color{white}:}{\color{magenta}Active}$|Get all active firewall zones.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Services}$|Get all services associated with the firewall.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Running}$|Check if the firewall is running.
|${\color{magenta}Firewall}{\color{white}:}{\color{magenta}Service}$|Check if a specific service is active in the firewall.




