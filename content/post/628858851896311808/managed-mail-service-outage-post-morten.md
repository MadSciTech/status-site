+++
title = 'Managed Mail Service Outage - Post-Morten'
date = 2020-09-10T00:01:15-05:00
+++
First off, I would like to apologize for this unexpected outage to our valued clients.

Our recent managed mail service outage that was between **12:17A - 12:35A on September 10, 2020**, was a result of a missed announcement of an upcoming maintenance window by our Data Center Provider to resolve an issue with the underlying server that our Managed Mail Service is hosted on. This maintenance window was missed due to multiple maintenance notices for the Month of September.

**The maintenance window was scheduled for**:

**Start**: 2020-09-10 @ 04:00 UTC / Sept 9, 2020 @ 11:00PM CDT
**End**: 2020-09-10 @ 12:00 UTC / Sept 10, 2020 @ 7:00AM CDT

Live migration was attempted, however, failed and an offline migration had to be performed. An offline migration requires the Managed Mail Server to be powered off before the migration process. This offline migration caused the outage and extended the downtime.

**Timeline of Events**:

* 12:17A - Data Center Provider Attempt Live Migration of Mail Server to the new host, but fails
* 12:22A - System Monitoring: Notification that Mail Server is unavailable
* 12:24A - Started investigating
* 12:28A - Found that Data Center is performing offline migration of Server
* 12:30A - Migration Completed
* 12:35A - Server back online

As mentioned above, there are other upcoming maintenance windows scheduled for September 2020, below is the upcoming maintenance windows:

* September 13, 2020 (CDT) - Hypervisor/Network Upgrades
* September 17, 2020 (CDT) - General Data Center Maintenance

Again, I would like to apologize again for this outage and I take full responsibility for this error.

If you have any questions or concerns, please feel free to [contact us](https://madscitech.com/about/contact/).

Chris Holbrook
Mad Scientist Technologies