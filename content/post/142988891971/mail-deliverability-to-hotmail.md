+++
title = 'Mail Deliverability to Hotmail'
date = 2016-04-18
+++
**[Open Issue]**

---

As of April 17, 2016 at 10:15PM CDT. We started recieved reports that email messages destined for Hotmail/Outlook.com email addresses were not being delivered to Hotmail/Outlook.com email accounts.

## Investigating

**April 17 @ 10:45PM**

We have confirmed the issue and we’re currently looking into the problem. We will update this page as soon as we have additional information to share.

## Working on it

**April 18 @ 1:00AM**

We have reached out to Microsoft, but we must wait for them to gather and report data back to us. This process may take up to 72 hours. We would like to apologize for this issue and the inconvenience this has caused our valued clients.

We will continue to see if we can resolve the problem from our side.

We will share more information as we get it.

**April 18 @ 6:00AM**

We may have found the problem. It seems that our configuration for DKIM verification may have an error in it. We are currently seeing what can be done to fix the issue, without reissuing DKIM Keys.

**April 18 @ 8:50AM**

The cause of the problem is caused by an configuration error on our DKIM configuration. Apparently when the server signed outgoing mail the domains’ DKIM it put the wrong DNS name to verify the DKIM key.

We will be rolling out a fix, shortly.

We will update this post with more information as it comes in.

**April 18 @ 11:30PM**

We have rekeyed our DKIM implementation and updated SPF Records for each client that is effected by this change. If we manage your DNS Records you have nothing to worry about, however if you manage your own DNS Records, we will be in contact with you to update your DKIM and SPF records.

As soon as these new DNS Records have propagated, we will be able to confirm that this issue is cleaned up.

We would like to apologize again for this issue and any inconvenience that it has caused you.

**April 19-20**

Update: We have discovered that Microsoft’s Hotmail.com, Outlook.com, and Live.com email accounts do not accept mail from _new or small email server_ and been a documented issue with Microsoft Email Service since 2010.

We will be reaching out to Microsoft to request an exception for our clients and our mail server. This process may take a few business days to sort out.

We will share more information as we receive it, stay tune.

We would like to apologize again for this issue.