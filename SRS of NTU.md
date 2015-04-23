
###Nautic Translate Update
###Requirements Specification Document

Date 11-september-2014


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
      * [**4.0	Client Requirements**](#iv-Client-Requirements)
      * [**5.0	System Specifications**](#v-system-specifications)
      * [**5.1	Internationalization**](#v-a-Internationalization)
      * [**5.2	Dictionary**](#v-b-dictionary)
      * [**5.3	Rate Screen**](#v-c-rate-screen)
      * [**5.4	Cashbox**](#v-d-cashbox)
      * [**6.0	Reference Screens**](#v-reference-screens)
      * [**7.0	Database Analysis**](#v-database-analysis)
      




#### (I) Introduction
 This document contains the system requirements for “Nautic Translate Application”. These requirements have been derived from several sources, including meetings with client, demos given to the client by Coeus Solutions .etc. 
“Nautic Translate Application” is a mobile application, it is intended to be used by the skipper of ship to take the advantage from a consolidated dictionary for nautical terms. Translations are available in German, Italian, Spanish, Turkish, Danish, Portuguese, Dutch and Greek for more than 1800 nautical terms of different categories.  
#### (II) Business Overview
From Business point of view this system will help to improve revenue of the company as skipper would be able to interact with different customers of different cultures and languages through fully consolidate dictionary. And also the functionality to manage the crew of the ship.
#### (III) Hardware or Software Requirements
The application should work on the following hardware and software.
* iPhone 6 + IOS 8
* Android XHDPI Resolution with latest OS.
#### (IV) Client Requirements
This is a list of Modules shared by the client on email/call.
|**Module Name**| **Comments**                     | 
|---------------|:------------------------------------- |
|Internationalization       | Application should be supported in 8 different languages .i.e German, Italian, Spanish, Turkish, Danish, Portuguese, Dutch and Greek |
|||
|Dictionary       |Categories, Sub-Categories and Detail Page                  | 
|||
|Rate Screen       |Rating of application              | 
|||
|Cashbox       |Create, Edit, Activate, Deactivate               | 

*note : Throughout application should work in Portrait mode.

#### (V) System Specifications
We have divided the Basic Flow of Ready2Serve POS in the following modules or specifications, let us evaluate them briefly through the concise description.

#### (V A) Internationalization

**User story title: sign in**       <br/>
As a **salesman/admin**        <br/>
I want to **sign in to the system**        <br/>
so that **I can use the fully functional system**       <br/>

|**S.No.**| **Pre-requisite**                     | **Acceptance criteria**             |**Status**|
|---------|:------------------------------------- |:------------------------------------|:--------:|
|1.       | salesman/admin has already an account | **When** the user requests to logIn | |
|         |**And**                                | **then**                            | |
|||||
|2.       |the user type his/her                  | ensure the account is activated     | |
|         |  valid username                       | And the control goes to main menu   | | 
|         |  valid password                       |                                     | |
|         |both consisting of varchar values	     |                                     | |
|||||
|3.       |And the user type his/her              | ensure the rejection message is displayed | |
|         |  valid username                       | And ensure user not logged in             | | 
|         |  Invalid password                     |  And prompt the user to reEnter.          | |
|         |both consisting of varchar values	     |                                           | |
|||||
|4.       |And the user type his/her              | ensure the rejection message is displayed | |
|         | Invalid username                      |   And ensure user not logged in           | |
|         | valid password                        | And prompt the user to reEnter.           | |
|         |Both consisting of varchar values      |                                           | |	 
|||||
|5.       |And the user type his/her              | ensure the rejection message is displayed | |     
|         | Invalid username                      |  And ensure user not logged in            | |
|         | Invalid password                      | And prompt the user to reEnter.	          | |
|         |Both consisting of varchar values      |                                           | | 	 




#### (V B) Dictionary
**User story title: Place Order**       <br/>
As a **salesman**        <br/>
I want **to place requested order for a customer**        <br/>
so that **I can generate an order for the customer and system would save this record**       <br/>

|**S.No.**| **Pre-requisite**                     | **Acceptance criteria**             |**Status**|
|---------|:------------------------------------- |:------------------------------------|:--------:|
|         |The list of items and deals is displayed on the screen | **When** the user requests to add order line item||
|         |**AND**                                |**Then**                             | |
|||||
|1.       |salesman enters the                    |	ensure that Console clear all its contents | |
|         | valid index no. of the item/deal      |AND again shows the list of items and deals||
|         | valid Quantity          |AND shows the current added order line item and prompts to add more  | |
|||||
|2.       |salesman enters the                    |ensure the rejection message is displayed | |
|         | valid index no. of the item/deal      |And prompt to reEnter the values.	         | |
|         | Invalid Quantity 	                    |                                           | |
|||||
|3.       |salesman enters the                    |ensure the rejection message is displayed  | |
|         | Invalid index no. of the item/deal    |And prompt to reEnter the values.	         | |
|         | Valid Quantity 	
|||||
|4.       |salesman enters the                    |ensure the rejection message is displayed  | | 
|         |Invalid index no. of the item/deal     |And prompt to reEnter the values.          | |
|         |Invalid Quantity 	                     |                                           | |
	

#### (V C) Rate Screen
**User story title: View Order just requested by the customer**       <br/>
As a **salesman**        <br/>
I want to **review the order and make changes in that requested order for a customer**        <br/>
so that **I can generate an accurate order for the customer to avoid trouble in future.**       <br/>

|**S.No.**| **Pre-requisite**                     | **Acceptance criteria**             |**Status**|
|---------|:------------------------------------- |:------------------------------------|:--------:|
|         |The salesman is logged in              |**When** the salesman requests to make changes in the order| |
|         |**AND**	                          |**Then**                                                   | |
||||| 
|1.       |The salesman just added an order line item|	ensure the system shows the proper menu for the different options of changes.	

#### (V D) Cashbox
**User story title: Change of quantity for an order line item**       <br/>
As a **salesman**        <br/>
I want to **make changes in the quantity of an order line item just requested by the customer**        <br/>
so that **I can generate an accurate order for the customer to avoid trouble in future.**       <br/>

|**S.No.**| **Pre-requisite**                     | **Acceptance criteria**             |**Status**|
|---------|:------------------------------------- |:------------------------------------|:--------:|
||The salesman is on the section to change quantity of an item/deal|**When** the user requests to change the quantity||
|         |**AND**	                          |**Then**                              | |
|||||
|1.       |The salesman enters the valid new quantity  |ensure the updation                | |
|         |                                            |AND prompt to make further changes | |	
|||||
|2.       |The salesman enters the Invalid new quantity|ensure the rejection message is displayed | |
|         |                                            |AND prompts to reEnter	| |

#### (VI) Database Analysis
The database system which we would use most preferably is the **MySQL**.  <br/>
“MySQL” have many good reasons to use in this project.  <br/> 
* Tested with a broad range of different compilers.
* Works on many different platforms.
* Provides transactional and nontransactional storage engines.
* Uses multi-layered server design with independent modules.
* Uses a very fast thread-based memory allocation system.
* Executes very fast joins using an optimized nested-loop join.
* Implements SQL functions using a highly optimized class library that should be as fast as possible.    <br/>

#### (V A) Entity Relationship Diagram
For the entity relationship diagram we have used the Chen one model as a standard. And we have used MS Visio to design that.  <br/>
It is the logical flow of our system just at the abstract level.  <br/>
 
![enter image description here](https://raw.github.com/RazaChohan/Experimentation-Repo/sanaNewBranch/diagrams/Extended-ERD.png)

Important point about this ERD is that there is a week entity “OrderLineItem” that’s why it has marked as double lined entity.   <br/>


#### (V B) Database Schema
 
Here is given all the tables which we will generate through a DBscript to store information about all related contents of the system.  <br/>
That script would be used by anyone to generate data base and its tables.  <br/> 

 ![enter image description here](https://raw.github.com/RazaChohan/Experimentation-Repo/sanaNewBranch/diagrams/Database%20Schema%20Diagram.png)

As we can see that there would be five tables in the DB schema of Ready2Serve POS.  <br/>

**Note:**
* In **person.person_type** the default values stored are **admin** and **sale**
* In **product.product_type** the default values stored are **deal** and **item**
* Default username for salesman is **sales_man** and for admin it is **admin_man**
* Default password for salesman is **sales123** and for admin it is **admin123**
