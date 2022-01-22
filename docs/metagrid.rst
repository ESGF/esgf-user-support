Metagrid (Beta): Introduction/FAQ
==========================

Metagrid: an introduction
-------------------------

Metagrid is a faceted search web application for use in ESGF data discovery.  Metagrid is the web application to replace the CoG web frontend.  Metagrid has many of the same search features and dataset information as was available in CoG.  The major distinction is that due to its Javascript platform based on ReactJS its able to present an improved user interaction experience.

Several new features
---------------------

* **Facet value free-text entry**  Users no longer must scroll through a long list of value names for models, experiments, variables, etc.  Instead, they can start typing the name and the Metagrid webapp will make a list of suggestions based on string pattern matching.
* **Saved searches** Save and re-run your search query at a later date
* **Shareable result links**  Hand off a link to colleagues to repeat your search

Metagrid awaits your feedback.  Please give a try for your ESGF data discovery needs.

Metagrid FAQ
------------

General
*******

    .. image:: images/Metagrod-shot.png

Q: Where should I start?

A: If you are unfamiliar with the interface, you may want to take a tour.  Click on the Blue Dot Question Mark icon in lower left corner of the page, then take the tour

Q: I would like to share some feedback of Meta



User accounts
*************

Q:  Can I use my existing ESGF account?

A:  Existing ESGF accounts are not compatible with Metagrid.  For now, *test* accounts are available.  You have the option to create a test account at the CEDA server or use credentials from GitHUb or your ORCID

Downloads
*********

Q:  Why doesn't the http download work?

A:  As ESGF is a distributed system, meaning that the data files are hosted and served from many independent servers, some of the servers have published their data using http links.  In the recent past (several years ago) this was not of concern for the major browsers (Chrome, Firefox).  More recently, the browsers have introduced a security feature to disable insecure content when linked from a secure page.  The consequence is that the http links provided from some servers are disabled by default.   The remedy is to adjust security/privacy settings for your broswer.  This change can be completed specifically for metagrid (Beta) by finding 

Q: Can I perform a Globus download using Metagrid?

A:  Not at present.  Access to Globus script downloads is coming soon.
