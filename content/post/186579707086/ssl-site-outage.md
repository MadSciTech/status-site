+++
title = 'SSL Site Outage'
date = 2019-07-27
+++
Starting at **11:00PM on July 26, 2019**, many of our online services became unavailable due to expired security certificates.

This issue was caused by a silently failing scheduled task that would normally renew the certificates automatically and a notification system failing to send warnings about the expiration of said certificates.

It came to our attention at **1:30AM July 27, 2019** that the services were unavailable, we remedy the issue by 1:40AM. We will be implementing additional safe guards to prevent this issue in the future.

We would like to deeply apologize for this problem.