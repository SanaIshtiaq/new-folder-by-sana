
###Nautic Translate Update
##Project Requirement Document


| Version |	Date |	Description |	Name	| Author |
--------- | ---- | ----------- | ---- | ------ |
| 1.0 |	01-04-2015 |	The Requirement and Specification document for NTU	| Nautic Translate Update	| Coeus |
| 1.1 |	08-04-2015 |	SRS after analysis for NTU	| Nautic Translate Update	| Coeus |



####Table of Contents
 * [Nautic Translate Update](#nautic-translate-update)
      * [**1.0	Introduction**](#i-introduction)
      * [**2.0	Business Overview**](#ii-business-overview)
      * [**3.0	Hardware or Software Requirements**](#iii-Hardware-or-Software-Requirements)
      * [**4.0	Client Requirements**](#iv-client-requirements)
      * [**5.0	System Specifications**](#v-system-specifications)
      * [**5.1	Internationalization**](#v-a-Internationalization)
      * [**5.2	Dictionary**](#v-b-dictionary)
      * [**5.3	Rate Screen**](#v-c-rate-screen)
      * [**5.4	Cashbox**](#v-d-cashbox)
      * [**6.0	Reference Screens**](#vi-reference-screens)
      * [**7.0	UseCase Diagram**](#vii-usecase-diagram)
      * [**8.0	Entity Relationship Diagram**](#vii-entity-relationship-diagram)
      * [**9.0	Database Analysis**](#ix-database-analysis)
      




#### (I) Introduction
 This document contains the system requirements for “Nautic Translate Application”. These requirements have been derived from several sources, including meetings with client, demos given to the client by Coeus Solutions .etc. 
“Nautic Translate Application” is a mobile application, it is intended to be used by the skipper of ship to take the advantage from a consolidated dictionary for nautical terms. Translations are available in German, Italian, Spanish, Turkish, Danish, Portuguese, Dutch and Greek for more than 1800 nautical terms of different categories.  
#### (II) Business Overview
From Business point of view this system will help to improve revenue of the company as skipper would be able to interact with different customers of different cultures and languages through fully consolidate dictionary. And also the functionality to manage the crew of the ship.
#### (III) Hardware or Software Requirements
The application should work on the following hardware and software.
* iPhone 6 + IOS 8
* Android XHDPI Resolution with latest OS. <br/>
#### (IV) Client Requirements
<br/>
This is a list of Modules shared by the client on email/call.

|**Module Name**| **Comments**                     | 
|---------------|:-------------------------------------: |
|Internationalization       | Application should be supported in 8 different languages |
| | .i.e German, Italian, Spanish, Turkish, Danish, Portuguese, Dutch and Greek |
|Dictionary | Categories, Sub-Categories and Detail Page | 
|Rate Screen | Rating of application  | 
|Cashbox  | Create, Edit, Activate, Deactivate | 

* note : Throughout application should work in Portrait mode.

#### (V) System Specifications
We have divided the Basic Flow of “Nautic Translate Application” in the following modules or specifications, let us evaluate them briefly through the concise description.

#### (V A) Internationalization

|**Use-Case name**| **Internationalization**                     | 
|---------------------------|:-------------------------------------:|
|**Stakeholder**            | Any crew member |
| **Brief Description**     |The application will support the following language. German, Italian, Spanish, Turkish, Danish, Portuguese, Dutch and Greek|
| **Pre-Conditions**        |The user has tapped on the icon of this application at his/her device and the application is active now|
| **Main Success Scenario** |1.	By default application should start with the language which user has set in device setting.|
| | 2.	User will able to change the application language through Language in main menu.|
| | 3.	In case of Android: when user selects the language, then application should re launch automatically and reverted to the language which user has selected.|
| **ALternative Flow**      |  At any time: |
| | click on back arrow at device will stop the further processing of system and will close the application|
| **Post Condition**        |  The user is on the home page of application                      |



#### (V B) Dictionary
|**Use-Case name**         | **Dictionary**                     | 
|--------------------------|:-------------------------------------:|
|**Stakeholder**           | Any crew member |
| **Brief Description**    |  User will be able to search for “nautical terms” and their meaning in dictionary in 8 different languages.  |
| **Pre-Conditions**        |The user has tapped on the “Dictionary” from main menu of the application|
| **Main Success Scenario** |1.	Dictionary should be in form of categories, sub-categories and detail Page |
| | 2.	When user will start typing the word to search, the system will show the suggestions|
| | 3.	User should be able to select any language to translate the word|
| **ALternative Flow**      |         2a.  When user tap on suggestions to scroll, the keyboard will  disappear|
| |       At any time: |
| |             click on back arrow at top will direct the user to previous page|
| **Post Condition**        |  The user is viewing the results of his/her search                       |

	

#### (V C) Rate Screen
|**Use-Case name**         | **Rate Screen**                     | 
|------------------------- |:-------------------------------------:|
|**Stakeholder**           | Any crew member |
| **Brief Description**    |When user starts the app, he/she will see the full screen banner with some options |
| **Pre-Conditions** |The user has tapped on the icon of this application at his/her device and the application is active now|
| **Main Success Scenario** | **Option at rate screen would be** |
| | 1.	Do not ask again |
| | 2.	Rate BAHAUS NAUTIC |
| | 3.	Proceed to Bahaus Nautic |
| **ALternative Flow**      |  1a.  Tap on this option will close the banner and rate screen will not appear again|
| | 2a. Tap on this option will direct the user to store rating screen|
| | 3a. Tap on this option will close the banner. But whenever user will come again to the app the rate screen will be shown again|
| | At any time: click on back arrow at top will direct the user to previous page|
| **Post Condition**        |  The user is on the home screen of app  |


#### (V D) Cashbox
The main purpose of this module is to create and maintain the common expense in during marina tour such as food, drinks, electricity usage .etc.

|**Use-Case name**           | **Cashbox Creation**                     | 
|----------------------------|:-------------------------------------:|
|**Stakeholder**             | Skipper |
| **Brief Description**        | the user will able to create their cashbox and in a cashbox user will able to add amount of cashbox, add participants and a skipper. |
| **Pre-Conditions**         | The user is on the Cashbox module |
| **Main Success Scenario**  | **For creating cashbox user will perform following actions:** |
| | 1.	Enter cashbox name |
| | 2.	Enter amount |
| | 3.	Select type of currency |
| | 4.	Add at least one participant or more if he wants ( There is no limitation ) |
| | 5.	Enter Skipper name ( Not Mandatory) |
| | 6.	After the above actions, user will tap on the “done” button |
| **ALternative Flow**       |  Application will show error message against each invalid action i.e. |
| | 4a. User try to add participant without their name |
| | 6a. User try to create cashbox without any participant name |
| | 6b. User try to create cashbox without entering the cashbox name |
| | 6c. User try create cashbox with name of numeric string. |
| | At any time: |
| | click on back arrow at top will direct the user to previous page|
| **Post Condition**        |  The application will prompt the user for confirmation. 
The information in the confirmation popup should be following: |
| | 1.	Cashbox name |
| | 2.	All participant with their name |
| | 3.	Skipper name, if added otherwise the skipper label should not be displayed |


|**Use-Case name**            | **Cashbox Listing**                     | 
|-----------------------------|:-------------------------------------:|
|**Stakeholder**              | Skipper |
| **Brief Description**       | All the cashbox which user has made should be enlisted here |
| **Pre-Conditions** | The user is on the Cashbox module |
| **Main Success Scenario**   | 1.	Each cashbox name is enlisted with status (Active/Inactive) |
| | 2.	The cashbox names are in descending order |
| | 3.	Upon tapping on cashbox name application redirects the user to its detail page |
| **ALternative Flow**        | 7a. At any time only one cashbox will be in “Active” state. It means all others would be in “Inactive” or “Completed” state |
| | At any time: |
| | click on back arrow at top will direct the user to previous page |
| **Post Condition**          |  The user is on the detail page of cashbox |



#### (VI) Reference Screens
Following screenshots are attached, illustrating the functional modules listed above <br/>

![enter image description here]( https://raw.githubusercontent.com/SanaIshtiaq/new-folder-by-sana/master/diagrams/123.png)
<br/>
![enter image description here](https://raw.githubusercontent.com/SanaIshtiaq/new-folder-by-sana/master/diagrams/456.png)
<br/>
![enter image description here]( https://raw.githubusercontent.com/SanaIshtiaq/new-folder-by-sana/master/diagrams/789.png)

#### (VII) UseCase Diagram

#### (VIII) Entity Relationship Diagram
For the entity relationship diagram we have used the Chen one model as a standard. And we have used MS Visio to design that.  <br/>
It is the logical flow of our system just at the abstract level.  <br/>

#### (IX) Database Schema
