+++
title = 'Implementation of SPF, DKIM, and DMARC for Managed Mail Services'
date = '2024-01-01'
aliases = ['/projects-status/spf-dkim-dmarc-project']
slug = '/original-dmarc-outline'
+++
**Project Status**: In Progress / Partial Delay

_Last Update: August 27, 2016_

The timeline for this project has slipped due to the more pressing issue of mail delivery issues to Outlook.com/Hotmail.com/Live.com.

The timeline below will need to be re-evaluated due this delay. However we are happy to report that the majority of our Managed Mail Only Clients have been completely migrated to a full SPF, DKIM and DMARC Implementation. We are still monitoring the DMARC reports for problems before implementing the Quarantine and Reject functionality.

---

TL;DR: We setup stuff to make imposter mail accounts a thing of the past. Scroll to the end of the article for the rollout schedule for your service(s).

We are planning to implement DMARC (Domain-based Message Authentication, Reporting & Conformance) Records across all our own and managed mail domains in the coming weeks.

**Why are you implementing DMARC and What is it?**

DMARC is an Internet Standard that is used to confirm that a email messages are truly from who it say it’s from. For example, when you a send email message to another mail server, the remote mail server can use DMARC records to confirm that your message is really from your mail server and not an imposter. If the message is not from the authorize mail server it will quarantine and send us reports on why it failed.

**Affected Clients**

This implementation process will take a few weeks to implement and should not cause too many problems for our managed mail customers.

Our clients that have both Managed Mail and Web Presences on the other hand will have a slower rollout. The reason is with DMARC you must know and list all authorized hosts that can send email on behalf of your domain. If you use Email Service Providers (such as MailChimp, Amazon Web Services - Simple Email Service, Campaign Monitor, etc), web forms that send emails, and then your actual mail accounts - all these source must be included in the set of records that make DMARC.

We will reach out to each our Managed Web Presence Clients individually to confirm issues will not arise during this process.

---

**Implementation Schedule**

Tentative Schedule for DKIM, SPF and DMARC Records Rollout

* June - Present: DMARC Monitoring
* Late September - December: Slow Ramp for Quarantine
* January 2017 - May 2017: Slow Ramp for Drop

As of June 2016, all properties managed and/or hosted by us has it respective DKIM,SPF and DMARC records implemented. The DMARC records are only set to monitoring for problems with mail delivery. We are planning on gathering more information about mail traffic flows, before switching DMARC records to Quarantine or Drop mail.

The rough plan is to start switching over to Quarantine before the end of 2016 and then implement Drop in Spring 2017.

However, some domains may be delayed or fast tracked depending on that domain’s particular mail flows.

If you have questions about this process, implementation, or any other questions, please feel free to reach out to us.

---

**Update 6/6/2016: The Schedule Below is No Longer Current and Will Be Updated Soon.**

~~The below is the tentative schedule for the implementation of DMARC on our managed services.~~

* ~~Managed Mail Clients - Some properties may ramp faster, depending reports~~
  * ~~April 18, 2016: Initial Records Set (Monitor Only)~~
  * ~~May 2, 2016: Set to Quarantine 1% of Email that does not conform.~~
  * ~~May 5, 2016: Quarantine 5%~~
  * ~~May 9, 2016: Quarantine 10%~~
  * ~~May 12, 2016: Quarantine 25%~~
  * ~~May 23, 2016: Quarantine 50%~~
  * ~~May 30, 2016: Quarantine 75%~~
  * ~~June 13, 2016: Quarantine All - Mid Point~~
  * ~~June 16, 2016: Reject 1%~~
  * ~~June 23, 2016: Reject 5%~~
  * ~~June 30, 2016: Reject 10%~~
  * ~~July 5, 2016: Reject 25%~~
  * ~~July 7, 2016: Reject 50%~~
  * ~~July 11, 2016: Reject 75%~~
  * ~~July 18, 2016: Reject All - Complete~~
* ~~Managed Web Presence & Mail Client - The ramp for these properties will be slower, depends on reports~~
  * ~~April 21, 2016: Initial Record Set (Monitor Only)~~
  * ~~May 5, 2016: Set to Quarantine 1% of Email that does not conform.~~
  * ~~May 12, 2016: Quarantine 5%~~
  * ~~May 19, 2016: Quarantine 10%~~
  * ~~May 26, 2016: Quarantine 25%~~
  * ~~June 2, 2016: Quarantine 50%~~
  * ~~June 6, 2016: Quarantine 75%~~
  * ~~June 9, 2016: Quarantine All - Mid Point~~
  * ~~June 20, 2016: Reject 1%~~
  * ~~June 23, 2016: Reject 5%~~
  * ~~June 27, 2016: Reject 10%~~
  * ~~June 30, 2016: Reject 25%~~
  * ~~July 7, 2016: Reject 50%~~
  * ~~July 14, 2016: Reject 75%~~
  * ~~July 21, 2016: Reject All - Complete~~

~~This schedule is tentative and may vary per client needs or results or the reporting mechanism of the DMARC Standard. We will report to each client when their implementation reach the following milestones:~~

   * ~~Quarantine 50%~~
   * ~~Quarantine All~~
   * ~~Reject 25%~~
   * ~~Reject 75%~~
   * ~~Reject All~~
