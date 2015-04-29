Introduction
============

This project provides a web-based dashboard for viewing CloudI environment settings and changing key parameters. It uses the JQuery and DataTables javascript libraries to provide an attractive display with minimal coding needed for different browswer dependencies.

Most screens in the application provide the ability to search for specific text and the ability to change the sort order by clicking on the column name.  In addition, you can specify the host name or address to monitor.  Specific notes for each main screen are listed below.

 
Service Summary
===============
This screen provides a summary of services running on a CloudI node. 

Clicking on a service will display buttons to:

* Remove the service
* Restart the service
* Show subscriptions for that service

This screen refreshes every 60 seconds.

Code Path
=========
This screen provides a list of the current code paths and the ability to add a new code path.

Clicking on a code path entry will display buttons to:

* Remove the selected path 

This screen refreshes every 60 seconds.

Nodes 
=====
This screen lists both the connected and disconnected CloudI nodes.

This screen refreshes every 60 seconds.

Logging
=======
This screen displays the current logging configuration and allows you to change some detailed log settings.

