+++
title = 'Managed Mail Service Outage'
date = 2025-02-16T14:50:43-06:00
draft = false
+++

**Resolved 2025-Feb-16 at 7:30PM**

Starting about 2:50PM we are experiencing an outage of our managed mail services. We are currently investigating and will update this post by 3:20PM CST Today.

_All Times are in US Central Standard Time_

## Updates

* 15:23 (3:23PM): Network Connectivity is currently lost to the server, we are still investigating the problem. Next update will be posted at 3:35PM.
* 15:33 (3:33PM): Network Connectivity has been restored, however the service is down because it unable to access the authentication server for user accounts. Will update again by 3:50PM. 
* 15:49 (3:49PM): We are investigating issue with our Private Connectivity between the mail server the authentication server. We are rolling out a possible fix now. Next Update will be at 4:15PM at the latest.
* 16:14 (4:14PM): We are attempting to recovery our private network between the servers. We will also be taking our managed web services for a brief time. Next update will be at 4:40PM.
* 17:00 (5:00PM): We have implemented a temporary fix, while we investigating the root cause of the failure to our private network at our data center. Additional Updates will be posted here.
* Final Update/Root Cause: As of 17:30 (5:30PM)

## Root Cause

On February 16 starting at 14:43PM CST our monitoring systems detected our managed mail server offline. Upon investigation we found the server had lost connectivity to Public (Internet) and Private Networks. During the investigation we found that there may be an undetected outage with our data center provider. We were able to get the server's Internet Connection back. However, the server's private network would not come back online. We changed the authentication system to use the public connection over an encrypted link to temporary allow the mail system to come back online. Upon investigating and testing the connection to the private network, network come back online. We reverted the change to the Authentication System back over to the private network.

We will continue to monitor the situation and update if things change.

---

We apologize for this outage, if you have any questions or concerns, please feel free to [contact us](https://madscitech.com/about/contact/).

Mad Scientist Technologies Team
