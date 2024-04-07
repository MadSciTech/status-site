+++
title = 'July 17 2017 - Network Outage Postmortem'
date = 2017-07-19
+++
On Monday, July 17, 2017, starting at 9:40 PM (CDT) our primary web server started to experience network connectivity loss. We immediately started troubleshooting the issue, we found that we couldn’t connect the server and the network path to the data center was unavailable.

We contacted our data center, provider. At 9:53 PM (CDT) we received confirmation that there is a network outage currently in process.

At 9:55 PM (CDT) our Managed Web Services came back online, slowly at first. By 10:10 PM (CDT) all services were back online and running normally.

The unofficial reason for this outage was a failure with a border gateway router in our data center provider’s facility. The data center provider has scheduled an upcoming maintenance window for July 25, 2017, between 02:00 - 04:00 UTC (July 24, 9 PM - July 25 11 PM).

Steps are already in place to attempt to prevent another outage along these lines.

We deeply apologize for this outage.

Services Effected: Websites and Web Applications.