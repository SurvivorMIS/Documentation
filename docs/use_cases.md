#SurvivorMIS Use Cases

##History  
The SurvivorMIS was built by the [Friends of Maiti Nepal](http://friendsofmaitinepal.org) team in partnership with [Maiti Nepal](http://www.maitinepal.org). Maiti Nepal is a grassroots organization that combats human trafficking of women and children. The SurvivorMIS was first built to meet Maiti Nepal's daily operational needs. However, the organization decided to build the SurvivorMIS n an open way so that all organizations that combat human trafficking can use a common set of terminology and tools.

##Problem Definition  
Organizations that combat human trafficking have a need to collect evidence and actionable information from the first interaction with a survivor until the moment they exit from care. The SurvivorMIS is structured to standardize and ease the information collection process for grassroots organizations working in this field. The SurvivorMIS allows functional groups to interact with the system. Each functional group has a different set of technical and informational needs as described in the following table. We define **the field** as a group of team members who are deployed for a short period, one day or less, to a location where they work in the community. **Satellite offices** are field locations that temporarily house survivors and begin providing primary services from the anti-trafficking organization. Note that not all organizations have satellite offices, but the flexibility remains in the system. Some teams deploy to the field from the central office. For example, a rescue team may deploy to the field to rescue victims from an exploitative situation. The central office is the location where the majority of services are delivered as well as the location where major organizational departments are housed. This is likely the location with the core management and ICT infrastructure. Finally we define external audiences as groups who do not have direct interaction with the client but require aggregate information.  

The following table describes the technical and informational needs of each functional group:  
<table style="border: 1px solid black;">
	<thead>
		<tr>
			<th colspan="4" style="text-align:center;"><b>Technical and Information Needs of Each Functional Group</b></th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td style="border: 1px solid black;"><b>The Field</b></td>
			<td style="border: 1px solid black;"><b>Satellite Offices</b></td>
			<td style="border: 1px solid black;"><b>Central Office</b></td>
			<td style="border: 1px solid black;"><b>External Audiences</b></td>
		</tr>
		<tr>
			<td style="border: 1px solid black;">
				<ul>
					<li>Secure Survivor Registration through Mobile Phone</li>
					<li>Access to Existing Survivor Information through Mobile Phone</li>
					<li>Voice/SMS/Email communication</li>
					<li>Emergency Response Activation</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">
				<ul>
					<li>Desktop access to information system (registration, review & data collection)</li>
					<li>Survivor Case Management (recording care, defining decisions and transferring for advanced service delivery)</li>
					<li>Voice/SMS/Email communication</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">
				<ul>
					<li>Desktop access to the information system (registration, review, data collection, & reporting)</li>
					<li>Robust reporting and aggregation of data from satellite offices and the field</li>
					<li>Survivor Case Management for long-term and advanced service delivery</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">
				<ul>
					<li>Reports based on aggregated data</li>
					<li>Research</li>
					<li>Metadata sharing</li>
					<li>Sharing stories on media and social media</li>
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4"><b>Examples</b></td>
		</tr>
		<tr>
			<td style="border: 1px solid black;">
				<ul>
					<li>Surveillance teams</li>
					<li>Rescue teams</li>
					<li>Grassroots community teams</li>
					<li>Awareness raising and outreach teams</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">
				<ul>
					<li>Transit Homes</li>
					<li>Acute Care providers such as hospitals</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">
				<ul>
					<li>Headquarters</li>
					<li>Rehabilitation Centers</li>
					<li>Long-term care facilities</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">
				<ul>
					<li>Donors</li>
					<li>Academic institutions</li>
					<li>Governments</li>
					<li>Other organizations</li>
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4"><b>Technology Needs</b></td>
		</tr>
		<tr>
			<td style="border: 1px solid black;">
				<ul>
					<li>Mobile phones with voice, SMS, data and email access</li>
					<li>Access to register survivors with the MIS through the browser or native application</li>
					<li>Backup paper data collection forms</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">
				<ul>
					<li>Desktop computers with printers</li>
					<li>Internet connection for access to the information system and email</li>
					<li>Backup paper data collection forms in case the information system is inaccessible</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">
				<ul>
					<li>Desktop computers with printers</li>
					<li>Internet connection for access to the information system and email</li>
					<li>3rd party aggregation software such as Microsoft Excel to meet the needs of external audiences</li>
					<li>Backup paper data collection forms in case the information system is inaccessible</li>
				</ul>
			</td>
			<td style="border: 1px solid black;">N/A</td>
		</tr>
	</tbody>
<table>

##Intended Audience  
The SurvivorMIS is built to be run at the point of care. In plain English, the system is used where the survivor is being served which is most often in an office or clinic setting. Version 1 of the SurvivorMIS is intended to be accessed through a laptop or desktop computer. Version 2 will focus on moving from the office to the field by integrating with mobile data collection tools. The software is available for download and implementation by any organization working in this space. Please [contact us](http://survivormis.com/#contact) if you are interested in running your own implementation or contributing to the SurvivorMIS.

##Use Case  
Shreya Shrestha created the foundation for the following use case descriptions in a consultancy in 2014. These use cases describe the flow of individuals at one of the offices. This section contains a high level overview with specific details and graphics below.

Steps:  
<img src="img/use_case_overview.svg" alt="Use Case Overview" height="300"/>


##SurvivorMIS Information Model  
The OpenMRS team has created clearly defined [information model](http://en.flossmanuals.net/openmrs-guide/openmrs-information-model/) that are appropriate for users to understand. This section describes how the SurvivorMIS has implemented that information model. 

**Persons**  
Every individual that interacts with the SurvivorMIS is stored as a **person**. Each person has a set of key attributes that are collected about them. These include name, gender, date of birth, and address. Every survivor is registered as a person in the system. Every user is also a person in the system, but they receive special user privileges and roles to be able to access the SurvivorMIS.

**Survivors and Patients**  
The SurvivorMIS is a module that adds functionality to the standard distribution of OpenMRS. We have tried to define different terminology across the system to distinguish between clinical and social services provided to the survivor. We have distinguished a different dashboard and set of data collection forms specific to the social services and separated them from the clinic. Survivors and patients are the same person in the system, but we expect that the term *survivor* is used by the team providing social services and the term *patient* is used by the clinicians providing clinical care.

**Registration**  
Each survivor who interacts with a team member must first register in the SurvivorMIS. This registration process creates a *person* record for the survivor. This process is activated by clicking the button labelled "Register a Survivor" in the home menu. Once registration is complete, the SurvivorMIS

**Visits**  
Once the survivor is registered, the team member must start a visit. A visit allows for the system to begin tracking services provided to the survivor at a particular location.

**Encounters** *(same as OpenMRS)*  
A moment in time where a survivor is seen by a provider at a location, and data is captured. Generally speaking, every time you enter a form in the SurvivorMIS, this creates an Encounter. For example, a visit with a legal section team member is an encounter between the survivor and the team member. Data collected in this event is tracked by the system as an encounter.

**Observations** *(same as OpenMRS)*  
An Observation is one single piece of information that is recorded about a person at a moment in time. Most observations happen in an encounter. Every observation has a Concept as its question, and depending on the datatype of the concept, it has a value that is a number, date, text, Concept, etc.

**Forms** *(same as OpenMRS)*   
A Form represents an electronic form that may be used for entering or viewing data. The SurvivorMIS metadata package provides the shared concepts, encounters and forms so organizations can begin collecting information with a minimal amount of customization.

**Concepts** *(same as OpenMRS)  
The most important part of the SurvivorMIS is the open source concept dictionary which is a list of all program related terms that will be used as questions and answers in Observations. The SurvivorMIS metadata package contains hundreds of terms that can be added to your concept dictionary to get your organization up and running quickly. An implementation can import the metadata package in a few minutes and the concepts, forms and encounter types are automatically created.

**Data** *(same as OpenMRS)*  
The actual information you want to record in the SurvivorMIS is called Data. Examples of data include the name of the survivor, date of birth, mother tongue, etc. To support the collection of this data, you need to create Metadata that provides the environment to begin collecting data.

**Metadata** *(same as OpenMRS)*  
Metadata is simply defined as the forms, fields and structure by which you collect information. The actual information that you collect about the survivor is data, but the form in which you collect that information is metadata. The SurvivorMIS comes with a metadata package the automatically imports concepts, forms, encounter types, roles, and privileges that allow your organization to get up and running quickly. These items are all metadata that provide structure to your implementation of the SurvivorMIS. We fully expect you to adjust these metadata fields to best meet the need of your organization. Please use [our contact form](http://www.survivormis.com#contact) if you would like to contribute to our metadata package by adding your implementation specific metadata.

**Users, Roles and Privileges** *(same as OpenMRS)*  
A User in the SurvivorMIS is an account that a person may use to log into the system.

The real-life person must be represented by a Person record in the SurvivorMIS, and a person may have more than one user account.

A Role represents a group of privileges in the system. Roles may inherit privileges from other roles, and Users may have one or more Roles.

A Privilege is an authorization to perform a particular action in the system. The list of available privileges are defined by the core system and by add-on modules (for example, Delete Survivors and Manage Encounter Types), but you need to configure which Roles have which Privileges while you are configuring your system. The SurvivorMIS metadata package contains numerous privileges and roles that allow administrators to ensure appropriate access controls at the user level. 

**Providers**  
A provider is the person who provides the care for the Survivor. Encounters can only be created by a person who has the provider role in the system. This is a feature that provides specific access control to a set of team members, ensuring that the encounter is captured by an authorized person.

