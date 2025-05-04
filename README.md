# server-scripts
Scripts for server management

## Firewall Functions
This section contains functions to manage the firewall on a server. The functions allow you to check the status of the firewall, manage firewall zones, and handle ports, protocols, and services associated with those zones.

|Name|Description|
| --- | --- |
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Active}$|Check if the firewall is active.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Inactive}$|Check if the firewall is inactive.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}$|Check if a specific firewall zone exists.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a specific firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Create}$|Create a new firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Source}$|Check if a source is associated with a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Source}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add a source to a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Source}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a source from a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Interface}$|Check if an interface is associated with a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Interfaces}$|Get all interfaces associated with a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Interface}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add an interface to a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Interface}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete an interface from a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Target}$|Set or get the target of a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Port}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add a port to a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Port}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a port from a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Ports}$|Get all ports associated with a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Protocols}$|List all protocols associated with a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Protocol}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add a protocol to a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Protocol}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a protocol from a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Services}$|Get all services associated with a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Service}{\color{#ffffff}:}{\color{#e11dbd}Add}$|Add a service to a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Service}{\color{#ffffff}:}{\color{#e11dbd}Delete}$|Delete a service from a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zone}{\color{#ffffff}:}{\color{#e11dbd}Service}$|Check if a specific service exists in a firewall zone.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zones}$|Get all firewall zones.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Zones}{\color{#ffffff}:}{\color{#e11dbd}Active}$|Get all active firewall zones.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Services}$|Get all services associated with the firewall.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Running}$|Check if the firewall is running.
|${\color{#e11dbd}Firewall}{\color{#ffffff}:}{\color{#e11dbd}Service}$|Check if a specific service is active in the firewall.

## Output Functions
This section contains functions to manage the output of scripts. The functions allow you to format and display messages in different styles, such as success, error, warning, info, debug, log, header, title, and summary.

|Name|Description|
| --- | --- |
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#42b20a}Success}$|Format and display a success message.
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#b20a0a}Error}$|Format and display an error message.
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#b2ac0a}Warning}$|Format and display a warning message.
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#3183da}Info}$|Format and display an informational message.
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#5ddd1d}Debug}$|Format and display a debug message.
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#e114c2}Log}$|Format and display a log message.
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#008aac}Header}$|Format and display a header message.
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#008aac}Title}$|Format and display a title message.
|${\color{#008aac}Output}{\color{#ffffff}:}{\color{#008aac}Summary}$|Format and display a summary message.

## Log Functions
This section contains functions to manage logging in scripts. The functions allow you to log stdout, stderr, and other messages.

|Name|Description|
| --- | --- |
|${\color{#c0b300}Output}{\color{#ffffff}:}{\color{#c0b300}Error}$|Log an error message.|
|${\color{#c0b300}Output}{\color{#ffffff}:}{\color{#c0b300}Output}$|Log standard output messages.|
|${\color{#c0b300}Output}{\color{#ffffff}:}{\color{#c0b300}Info}$|Log informational messages.|

## Ubuntu Functions
This section contains functions specific to Ubuntu systems. The functions allow you to manage the system, including checking the system's architecture, updating the system, and managing services.

|Name|Description|
| --- | --- |
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Auto}$|Check if a package is automatically installed (not manually installed) using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Available}$|Check if a package is available for installation using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Broken}$|Check if a package is broken (not properly installed) using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Clean}$|Clean up the local repository of retrieved package files using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Configure}$|Configure a package to set it up after installation using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Configured}$|Check if a package is configured (installed and set up) using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Configuring}$|Check if a package is currently being configured using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Held}$|Check if a package is held (not upgradable) using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Hold}$|Hold a package to prevent it from being upgraded using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Holding}$|Check if a package is currently being held (not upgradable) using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Install}$|Install a package using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Installed}$|Check if a package is installed using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Installing}$|Check if a package is currently being installed using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Manual}$|Check if a package is manually installed using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Purge}$|Purge a package to completely remove it from the system using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Purged}$|Check if a package is purged (completely removed) using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Purging}$|Check if a package is currently being purged using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Remove}$|Remove a package using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Removing}$|Check if a package is currently being removed using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Unhold}$|Unhold a package to allow it to be upgraded using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Update}$|Update the package list using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Upgradable}$|Check if a package is upgradable using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Upgrade}{\color{#ffffff}:}{\color{#ff7f00}Package}$|Upgrade a specific package using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Upgrade}$|Upgrade installed packages using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Apt}{\color{#ffffff}:}{\color{#ff7f00}Upgrading}$|Check if a package is currently being upgraded using Apt.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Command}{\color{#ffffff}:}{\color{#ff7f00}Available}$|Check if a command is available on Ubuntu.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Command}$|Run a command on Ubuntu.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Jammy}$|Check if the system is running Ubuntu Jammy (22.04).
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Noble}$|Check if the system is running Ubuntu Noble (24.04).
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Create}$|Create a systemd service file on Ubuntu.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Disable}$|Disable a service from starting at boot time.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Disabled}$|Check if a service is disabled from starting at boot time.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Enable}$|Enable a service to start at boot time.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Enabled}$|Check if a service is enabled to start at boot time.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Mask}$|Mask a service to prevent it from being started.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Masked}$|Check if a service is masked (disabled and cannot be started).
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Restart}$|Restart a service on the system.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Running}$|Check if a service is running on the system.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Start}$|Start a service on the system.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Stop}$|Stop a service on the system.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Service}{\color{#ffffff}:}{\color{#ff7f00}Unmask}$|Unmask a service to allow it to be started again.
|${\color{#ff7f00}Ubuntu}{\color{#ffffff}:}{\color{#ff7f00}Services}{\color{#ffffff}:}{\color{#ff7f00}Reload}$|Reload the systemd manager configuration on Ubuntu.
