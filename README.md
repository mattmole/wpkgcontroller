# WPKG-Controller

**Web based configuration and reporting software for WPKG**

As stated by http://www.wpkg.org:

> WPKG is an automated software deployment, upgrade and removal program for Windows.

> It can be used to push/pull software packages, such as Service Packs, hotfixes, or program installations from a central server (for example, Samba or Active Directory) to a number of workstations.

> It can run as a service to install software in the background (silent install), without user interaction.

> It can install MSI, InstallShield, PackagefortheWeb, Inno Setup, Nullsoft, other software installers or .exe packages, .bat and .cmd scripts and similar: no more repackaging to perform software installation. 

WPKG uses XML files to configure package, profile and host definitions. Also, the local state of package installations is stored on each client, in XML format.

WPKG-Controller is designed to:

* Allow configuration of hosts, profiles and packages in a simple to use, web-based GUI
* Uses database relationships to provide pull down options where appropriate in the aforementioned configuration
* Generate XML files which WPKG on each client can access
* Provide reports of package install priority within each profile / host definition
* Provide a grid view to see the installation status of each package and client
* If possible, provide a grid view, which allows host and package relationships to be set

Coding is carried out in Python, using the Django framework. Python version currently in use is 2.7.8 and Django version is 1.6.6.
