+++
title = 'Outage: DNS Failure at Provider'
date = 2016-03-24
+++
_March 24, 2016 @ 10:24AM_

Our Datacenter provider has reported that they are having problems with connections to their DNS Servers and are current investigating the problem.

Our servers are still online, but with DNS unavailable connections/clients may be unable to connect to the site.

We will update this post with more details, as soon as we have more details.

---

_March 24, 2016 @ 10:45AM_

Our Datacenter provider has identity the failure and are working to resolve the connectivity issue their DNS Servers.

_March 24, 2016 @ 11:45AM_

DNS services have been partially restored, we will continue to monitor the situation and update.

_March 24, 2016 - Postmortem_

Our New York Data Center Provider has posted an postmortem of the cause of today’s DNS failure. The cause was due to a increase demand upon their DNS Servers Clusters - Distributed Denial of Service Attack upon the providers DNS Infrastructure. The provider will be changing their DNS Infrastructure to improve the time to mitigate DNS DDoS Attack in the future.

If you have questions, please feel free to [reach out to us](https://madscitech.com/about/contact/).