---
date: 2014-08-27
title: Notice about a user data leak from landfill.bugzilla.org
---

Some email addresses and encrypted passwords for test builds on landfill.bugzilla.org were temporarily posted on a publicly accessible server.

One of our developers discovered that, starting on about May 4th, 2014, for a period of around 3 months, during the migration of our testing server for test builds of the Bugzilla software, database dump files containing email addresses and encrypted passwords were posted on a publicly accessible server. This resulted in the accidental disclosure of the email addresses and encrypted passwords of about 97,000 users. As soon as we became aware, the database dump files were removed from the server immediately, and we’ve modified the testing process to not require the database dumps.

More detailed information can be obtained from the [Bugzilla Blog](https://bugzillaupdate.wordpress.com/2014/08/27/landfill-bugzilla-org-disclosure/)

