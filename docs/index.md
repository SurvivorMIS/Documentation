========
Overview
========

Welcome to the SurvivorMIS!

This document is a brief explanation of the purpose, workflow and outcomes associated with the SurvivorMIS. Additional documentation will soon be available.

What is the SurvivorMIS?
========================

The Survivor Management Information System is a point of care information system custom tailored to support the care, rehabilitation and recovery of survivors of domestic violence, rape and human trafficking. The SurvivorMIS is built using world-class open source technology. Most importantly, the team is developing the first open source concept dictionary that exclusively focuses on domestic violence, rape and human trafficking. This dictionary cuts across commonly siloed services such as police, justice and health.

More specifically, the SurvivorMIS is:  
* A module that adds a Survivor dashboard to the OpenMRS 2.x reference application;  
* An open source set of metadata forms, questions and fields that allow organizations care for survivors of domestic violence, rape and human trafficking  

Installation
============
The module currently needs to be built from source to be deployed. Like other openMRS modules, this is built with the maven archetype. 
1) Clone this repository in eclipse or IntelliJ  
2) Maven build 'clean install'
3) Copy the resulting omod should be copied to the openMRS modules folder

Next, you must download the latest zip file of the metadata from the `openmrs-metadata-SurvivorMIS` repository. This file should be uploaded using the Metadata Sharing module of OpenMRS.  
1) Click Import Metadata  
2) Click Import Package  
3) Upload the zip file  
4) Click Next until you get to review the data  
5) The metadata contains copies of a few CIEL concepts. You can overwrite your dictionary if you feel it's appropriate  

Important Links
===============
The source code is available in the [github.com/SurvivorMIS](https://github.com/SurvivorMIS/) account.  
We use the github issue trackers for each repository to track issues to the [module](https://github.com/SurvivorMIS/openmrs-module-SurvivorMIS/issues) and [metadata](https://github.com/SurvivorMIS/openmrs-metadata-SurvivorMIS/issues).  
Please complete the contact form at [SurvivorMIS.com](http://suriviormis.com) to contact our team.  

Troubleshooting
===============
The biggest issue has to do with incorrectly loading the metadata. All references in the HTMLForms point to a mapped version of each concept (i.e. "SurvivorMIS:162223"). The HTMLForm will not load if a concept is incorrectly mapped. Please let us know if there is an issue the first time you load the metadata.  

Loading multiple versions of the metadata should be done on updates and when issues close. Follow the same steps to load the data choosing "Master" as the source. Note that you should not change existing concepts if they match exactly.
