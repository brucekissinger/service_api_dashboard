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

View Log File
=============
This screen displays the current log file contents with a filter for different log levels.  The screen refreshes every 60 seconds.

Note that in order to use this function, there MUST be an entry in the cloudi.conf similar to what is shown below.

        % Used for viewing logs on the Dashboard
        {internal,
                "/dashboard/log/",
                cloudi_service_filesystem,
                [{directory, "/usr/local/var/log/cloudi"},
                {refresh, 60},          % 1 minute
                {cache, 60},            % 1 minute
                {use_http_get_suffix, true}],      
                none,
                60000, 5000, 5000, [api], undefined, 1, 1, 300, []}


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

Log Settings
============
This screen displays the current logging configuration and allows you to change some detailed log settings.

