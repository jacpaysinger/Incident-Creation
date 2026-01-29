# Incident Creation Using Classic Lists and Forms

## Overview
This repository demonstrates how to create, update, and locate Incidents using the classic ServiceNow interface. The focus is on practicing core ITSM navigation, documenting incidents accurately, and validating records through classic lists and group-based work views.

The implementation reflects a real-world support scenario where an end user reports an urgent application issue and a service desk analyst captures, documents, and routes the incident appropriately.

## Use Case
A staff member relies on a mobile application to support a time-sensitive business event. When the application fails to launch and displays an error, the issue must be recorded quickly and accurately so it can be routed to the correct support team.

This project simulates the incident creation and validation process from an end-user perspective and demonstrates how classic lists, forms, and work queues are used in day-to-day IT service operations.

## Features
- User impersonation to validate the end-user experience
- Incident creation using classic lists and forms
- Population of service, offering, and configuration item fields
- Separation of internal work notes and customer-visible comments
- Incident validation using History and list navigation
- Review of group-based work assignments

## Technologies Used
- ServiceNow Platform
- IT Service Management (ITSM)
- Incident Management
- Classic Lists and Forms
- User Impersonation

## Implementation Walkthrough

### Objective
Create, document, and validate an Incident in the classic ServiceNow environment while demonstrating effective navigation and record management techniques.

### Step 1: Impersonate the End User
The user menu was used to impersonate an end user to ensure the workflow reflected a realistic user experience rather than administrator access.

**Impersonated User**
- Beth Anglin

Visual indicators confirmed the instance was operating in an impersonated session.

### Step 2: Navigate to Incident Creation
A new Incident was created using the classic interface.

Navigation path:
- All > Incident > Create New

### Step 3: Create the Incident Record
The Incident form was completed with the following information:

- Caller: Fred Luddy  
- Category: Software  
- Subcategory: None  
- Short description: Cannot get the Conference Event Mobile app for staff to launch. It is flashing error 555.  
- Description: It was working yesterday, but not this morning. This is urgent. The event starts in 3 hours.

### Step 4: Define Service Context
To accurately associate the incident with business services, the following fields were populated:

- Service: Conference Event Services  
- Service Offering: Event Mobile for Staff Service Offering  
- Configuration Item: Event Mobile for Staff Application  

This ensures proper routing, reporting, and SLA tracking.

### Step 5: Complete Incident Details
Additional incident attributes were reviewed or set as follows:

- Channel: Phone  
- State: New  
- Impact: 1 – High  
- Urgency: 1 – High  
- Priority: Automatically calculated as 1 – Critical
  
The record was saved without submitting to remain on the form.

<img width="1815" height="545" alt="Screen Shot 2026-01-28 at 6 23 57 PM" src="https://github.com/user-attachments/assets/b4f44289-f8ba-4084-8563-3bb1d9e3564b" />


### Step 6: Add Work Notes and Customer Comments
The Notes tab was used to document both internal and customer-facing updates.

- Work notes: No outages have been reported, am routing to the Conference Event App support team.  
- Additional comments: Fred, we are working on getting the app up and running.
  
This demonstrates the separation between internal documentation and customer communication.

<img width="1815" height="823" alt="Screen Shot 2026-01-28 at 6 26 22 PM" src="https://github.com/user-attachments/assets/f8a13518-18f7-4846-8845-68daf92f5817" />


### Step 7: Review Incident Activity and Related Records
The History menu was used to reopen the Incident. The Activity stream was reviewed to confirm that notes, comments, and timestamps were recorded correctly.

Related Lists were reviewed to observe associated records such as:
- SLA timelines
- Impacted services
- Service offerings

### Step 8: Capture the Incident Number
The Incident number was recorded to support quick retrieval using list searches.

### Step 9: Navigate to Open Incidents
The Open Incidents list was accessed using:

- All > Incident > Open

### Step 10: Locate the Incident Using List Tools
The Incident was located using multiple list techniques:
- Sorting the Opened column
- Searching the Number column using the full Incident number
- Using wildcard searches to locate partial values
  
These techniques demonstrate efficient navigation within large record sets.

<img width="1815" height="326" alt="Screen Shot 2026-01-28 at 6 56 20 PM" src="https://github.com/user-attachments/assets/df26bd21-9f2e-49e2-ad85-953141bde874" />

### Step 11: Access Service Desk Modules
The Service Desk module was accessed from the All menu.

### Step 12: Add My Groups Work to Favorites
The My Groups Work module was added to Favorites to allow quick access to group-assigned records.

### Step 13: Open My Groups Work from Favorites
The Favorites menu was used to open Service Desk – My Groups Work.

The list header and breadcrumbs were reviewed to confirm:
- The correct table was displayed
- Filters were applied to show unassigned group work

This view demonstrates how analysts monitor incoming work before individual assignment.

<img width="1815" height="326" alt="Screen Shot 2026-01-28 at 6 29 58 PM" src="https://github.com/user-attachments/assets/646449ee-ca92-4038-ae5e-67a50703a97e" />



## Lessons Learned
- User impersonation is critical for validating realistic user experiences
- Classic lists and forms remain foundational to ITSM workflows
- Accurate service context improves routing and SLA tracking
- Work notes and additional comments serve distinct communication purposes
- Group-based work views support effective workload management
