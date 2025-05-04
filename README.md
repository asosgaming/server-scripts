# server-scripts
Scripts for server management

## ${\color{#e11dbd}Firewall\ Functions}$
This section contains functions to manage the firewall on a server. The functions allow you to check the status of the firewall, manage firewall zones, and handle ports, protocols, and services associated with those zones.

|Name|Description|Arguments|
| --- | --- | --- |
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Active}$|Check if the firewall is active.|
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Inactive}$|Check if the firewall is inactive.|
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}$|Check if a specific firewall zone exists.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a specific firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Create}$|Create a new firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Source}$|Check if a source is associated with a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_source}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Source}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add a source to a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_source}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Source}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a source from a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_source}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Interface}$|Check if an interface is associated with a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_interface}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Interfaces}$|Get all interfaces associated with a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Interface}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add an interface to a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_interface}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Interface}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete an interface from a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_interface}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Target}$|Set or get the target of a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_target}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Port}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add a port to a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_port}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Port}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a port from a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_port}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Ports}$|Get all ports associated with a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Protocols}$|List all protocols associated with a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Protocol}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add a protocol to a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_protocol}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Protocol}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a protocol from a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_protocol}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Services}$|Get all services associated with a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Service}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add a service to a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_service}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Service}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a service from a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_service}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Service}$|Check if a specific service exists in a firewall zone.|${\color{#ffffff}<}{\color{#9f790f}zone\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}zone\_service}{\color{#ffffff}>}$
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zones}$|Get all firewall zones.|
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zones}{\color{#ffffff}:}{\color{#e11dbd}Active}$|Get all active firewall zones.|
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Services}$|Get all services associated with the firewall.|
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Running}$|Check if the firewall is running.|
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Service}$|Check if a specific service is active in the firewall.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$

## ${\color{#008aac}Output\ Functions}$
This section contains functions to manage the output of scripts. The functions allow you to format and display messages in different styles, such as success, error, warning, info, debug, log, header, title, and summary.

|Name|Description|Arguments|
| --- | --- | --- |
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#42b20a}Success}$|Format and display a success message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#b20a0a}Error}$|Format and display an error message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#b2ac0a}Warning}$|Format and display a warning message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#3183da}Info}$|Format and display an informational message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#5ddd1d}Debug}$|Format and display a debug message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#e114c2}Log}$|Format and display a log message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#008aac}Header}$|Format and display a header message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#008aac}Title}$|Format and display a title message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#008aac}Summary}$|Format and display a summary message.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$

## ${\color{#c0b300}Log\ Functions}$
This section contains functions to manage logging in scripts. The functions allow you to log stdout, stderr, and other messages.

|Name|Description|Arguments|
| --- | --- | --- |
|${\color{#c0b300}Output}{\color{#ffffff}:}{\color{#c0b300}Error}$|Log an error message.|2> >(Log:Error)
|${\color{#c0b300}Output}{\color{#ffffff}:}{\color{#c0b300}Output}$|Log standard output messages.|> >(Log:Output)
|${\color{#c0b300}Output}{\color{#ffffff}:}{\color{#c0b300}Info}$|Log informational messages.|${\color{#ffffff}<}{\color{#9f790f}message}{\color{#ffffff}>}$

## ${\color{#ff7f00}Ubuntu\ Functions}$
This section contains functions specific to Ubuntu systems. The functions allow you to manage the system, including checking the system's architecture, updating the system, and managing services.

|Name|Description|Arguments|
| --- | --- | --- |
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Auto}$|Check if a package is automatically installed (not manually installed) using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Available}$|Check if a package is available for installation using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Broken}$|Check if a package is broken (not properly installed) using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Clean}$|Clean up the local repository of retrieved package files using Apt.|
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Configure}$|Configure a package to set it up after installation using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Configured}$|Check if a package is configured (installed and set up) using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Configuring}$|Check if a package is currently being configured using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Held}$|Check if a package is held (not upgradable) using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Hold}$|Hold a package to prevent it from being upgraded using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Holding}$|Check if a package is currently being held (not upgradable) using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Install}$|Install a package using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Installed}$|Check if a package is installed using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Installing}$|Check if a package is currently being installed using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Manual}$|Check if a package is manually installed using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Purge}$|Purge a package to completely remove it from the system using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Purged}$|Check if a package is purged (completely removed) using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Purging}$|Check if a package is currently being purged using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Remove}$|Remove a package using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Removing}$|Check if a package is currently being removed using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Unhold}$|Unhold a package to allow it to be upgraded using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Update}$|Update the package list using Apt.|
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Upgradable}$|Check if a package is upgradable using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Upgrade}{\color{#ffffff}:}{\color{#ff7f00}Package}$|Upgrade a specific package using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Upgrade}$|Upgrade installed packages using Apt.|
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Upgrading}$|Check if a package is currently being upgraded using Apt.|${\color{#ffffff}<}{\color{#9f790f}package\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Command}{\color{#ffffff}:}{\color{#ff7f00}Available}$|Check if a command is available on Ubuntu.|${\color{#ffffff}<}{\color{#9f790f}command\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Command}$|Run a command on Ubuntu.|${\color{#ffffff}<}{\color{#9f790f}command\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}arguments}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Jammy}$|Check if the system is running Ubuntu Jammy (22.04).|
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Noble}$|Check if the system is running Ubuntu Noble (24.04).|
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Create}$|Create a systemd service file on Ubuntu.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}service\_description}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}service\_command}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Disable}$|Disable a service from starting at boot time.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Disabled}$|Check if a service is disabled from starting at boot time.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Enable}$|Enable a service to start at boot time.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Enabled}$|Check if a service is enabled to start at boot time.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Mask}$|Mask a service to prevent it from being started.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Masked}$|Check if a service is masked (disabled and cannot be started).|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Restart}$|Restart a service on the system.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Running}$|Check if a service is running on the system.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Start}$|Start a service on the system.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Stop}$|Stop a service on the system.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Unmask}$|Unmask a service to allow it to be started again.|${\color{#ffffff}<}{\color{#9f790f}service\_name}{\color{#ffffff}>}$
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Services}{\color{#ffffff}:}{\color{#ff7f00}Reload}$|Reload the systemd manager configuration on Ubuntu.|

## ${\color{#1d68e1}File\ Functions}$
This section contains functions specific to file management. The functions allow you to set permissions, flags, and retrieve file system information.

|Name|Description|Arguments|
| --- | --- | --- |
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Create}{\color{#ffffff}:}{\color{#1d68e1}Empty}$|Create an empty file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Create}$|Create a new file or directory.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}directory}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Delete}$|Delete a file or directory.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Directory}$|Check if a file is a directory.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Executable}$|Check if a file is executable.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Exists}$|Check if a file or directory exists.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}ACL}$|Get the Access Control List (ACL) of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Device}$|Get the device number of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}ExtendedAttributes}$|Get the extended attributes of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Filesystem}$|Get the filesystem type of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Flags}$|Get the flags of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}FreeInodes}$|Get the free inodes available on the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}FreeSpace}$|Get the free space available on the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Group}$|Get the group of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Inode}$|Get the inode number of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Inodes}$|Get the inode usage statistics of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Label}$|Get the label of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}MountOptions}$|Get the mount options of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}MountPoint}$|Get the mount point of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Owner}$|Get the owner of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Permissions}$|Get the permissions of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}SecurityLabel}$|Get the security label of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}SELinuxContext}$|Get the SELinux context of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Symlink}$|Get the target of a symbolic link.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}TotalInodes}$|Get the total inodes of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}TotalSpace}$|Get the total space of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Type}$|Get the type of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}Usage}$|Get the usage statistics of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}UsedInodes}$|Get the used inodes of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}UsedSpace}$|Get the used space of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Get}{\color{#ffffff}:}{\color{#1d68e1}UUID}$|Get the UUID of the filesystem containing a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Immutable}$|Check if a file is immutable (cannot be modified).|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Modified}$|Get the last modified time of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Readable}$|Check if a file is readable.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Regular}$|Check if a file is a regular file (not a directory or special file).|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}AccessTime}$|Set the access time of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}access\_time}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}ACL}$|Set the Access Control List (ACL) of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}acl}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}ChangeTime}$|Set the change time of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}change\_time}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}ExtendedAttributes}$|Set the extended attributes of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}extended\_attributes}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}Flags}$|Set the flags of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}flags}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}Immutable}$|Set a file as immutable (cannot be modified).|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}ModificationTime}$|Set the modification time of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}modification\_time}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}Owner}$|Set the owner of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}owner}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}Permissions}$|Set the permissions of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}permissions}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}SecurityLabel}$|Set the security label of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}security\_label}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Set}{\color{#ffffff}:}{\color{#1d68e1}SELinuxContext}$|Set the SELinux context of a file.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}\ {\color{#ffffff}<}{\color{#9f790f}selinux\_context}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Size}$|Get the size of a file in bytes.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}SymbolicLink}$|Check if a file is a symbolic link.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Unset}{\color{#ffffff}:}{\color{#1d68e1}Immutable}$|Unset the immutable flag of a file (allow modifications).|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$
|${\color{#1d68e1}File}{\color{#ffffff}:}{\color{#1d68e1}Writable}$|Check if a file is writable.|${\color{#ffffff}<}{\color{#9f790f}file\_path}{\color{#ffffff}>}$


