Metagrid (Beta): Introduction/FAQ
==========================

Metagrid: an introduction
-------------------------

Metagrid is a faceted search web application for use in ESGF data discovery.  Metagrid is the web application to replace the CoG web frontend.  Metagrid has many of the same search features and dataset information as was available in CoG.  The major distinction is that due to Metagrid's use of a Javascript platform based on ReactJS, Metagrid is able to present an improved interactive user experience.

Several new features
---------------------

* **Facet value free-text entry**:  Users no longer must scroll through a long list of value names for models, experiments, variables, etc.  Instead, they can start typing the name and the Metagrid webapp will make a list of suggestions based on string pattern matching.
* **Saved searches**: Save and re-run your search query at a later date on a different browser or system.
* **Shareable result links**:  Hand a link off to your colleagues to repeat your search

In addition, Metagrid addresses a long-standing issue that has impacted the CoG web frontend's ability to deliver the "Wget Script".  Download of the script with specific browser versions would produce a script with incorrect files.  To our knowledge this is no longer an issue for Metagrid.

Metagrid awaits your feedback.  Please give this interface a try for your ESGF data discovery needs.

Metagrid FAQ
------------

General
*******

Q: Where should I start with getting to know the Metagrid user interface?  I'm fairly new to ESGF and this all seems so unfamiliar?

A: If you are unfamiliar with the interface, you may want to take a tour.  Click on the Blue Question Mark icon in lower right corner of the page, then click on the available tour for your current page.

Q: I would like to share some feedback of Metagrid.  Is there an easy way to do so?

A: We have integrated HotJar into Metagrid to collect feedback.  Locate the gray tab in the lower-right corner of the page.  The HotJar popup window will ask a series of questions. The freetext answer fields are optional so can be skipped with the "Skip" link, but answers to the questions on a scale of 0-10 are required to complete the short survey. 

For more specific suggestion: bug reports, feature requests, etc., please open an issue on the Metagrid GitHub repo:  https://github.com/aims-group/metagrid/issues

   .. image:: images/Metagrid-shot.png

Q: How can I find Cordex data. It is not listed under projects.

A: For the time being Cordex data can be found under the last listed project All (except CMIP6)

Q: Why exclude CMIP6 from all other projects

A: CMIP6 introduced a different naming convention for several of the properties of the datasets in our search database, such as the model and experiment.  As we have been unable to reconcile the old and new conventions trivially, instead we provide results on separate pages.  
We realize this may pose an inconvenince to comparing data between older project data.  

Search
******

Q:  How do I include/exclude replicas in my search and search for old versions?

A:  The fields to toggle replicas and versions is under the **Additional Properties** Tab of the Faceted search bar on the left.


User accounts
*************

Q:  Can I use my existing ESGF account?

A:  Existing ESGF accounts are not compatible with Metagrid.  For now, *test* accounts are available.  You have the option to create a test account at the CEDA server or use credentials from GitHUb or your ORCID

Downloads
*********

Q:  Why doesn't my Http download work in Chrome?

A:  As ESGF is a distributed system, meaning that the data files are hosted and served from many independent servers, some of the servers have published their data using http links (as opposed to secure https links).  Such links are listed in the search results without modification.  In the recent past (several years ago) this arrangement was not of concern for the major browsers (Chrome, Firefox).  somewhat recently, the browsers have introduced a security feature to disable insecure content when linked from a secure page.  The consequence is that the http links provided from some servers are disabled by default.   The remedy is to adjust security/privacy settings for your broswer.

For Chrome users, you will need to go to your Settings -> Security & Privacy -> Site Settings -> Additional Content Settings -> Insecure content.  **Add** a site (using the button) to add ``aims2.llnl.gov`` to your list of sites.  That site execption will enable the downloads to proceed.

Q: Can I perform a Globus download using Metagrid?

A:  Not at present.  Access to Globus script downloads is coming soon.
