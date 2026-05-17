# Day 3 - Data Modeling and Validation

## What is Data Modeling?
Data modeling in Salesforce is the process of organizing business data using objects, fields, records, and relationships. It helps structure data in a way that makes business processes easy to manage.

## App vs Object vs Record vs Field

### App
An app is a collection of related tabs, objects, and tools used for a specific business purpose.

Example:
College Admission Management App

### Object
An object is like a database table that stores similar types of information.

Examples:
- Student
- Admission Application
- Department
- Faculty

### Record
A record is a single entry inside an object.

Example:
Student Name: Sreeja Mutha

### Field
A field stores specific information inside a record.

Examples:
- Student Name
- Email
- Phone Number
- Admission Status


## Standard vs Custom Objects

### Standard Objects
These are prebuilt Salesforce objects.

Examples:
- Account
- Contact
- Opportunity
- Contract

### Custom Objects
These are user-created objects based on business requirements.

Examples created in Day 3:
- Property
- Offer
- Favorite


## Relationships in Salesforce
Relationships connect objects together.

### Master-Detail Relationship
A strong relationship where child records depend on parent records.

Example:
Property → Offer

### Lookup Relationship
A looser relationship between objects.

Example:
Offer → Contact


## Formula Fields
Formula fields automatically calculate values.

Example completed:
Contract object formula field:

Days Remaining = End Date - TODAY()

This calculates how many days remain before contract expiration.


## Validation Rules
Validation rules prevent invalid data entry.

Example completed:
A contact cannot be saved if the contact ZIP code does not match the associated account shipping ZIP code.

Formula used:

AND(
NOT(ISBLANK(AccountId)),
MailingPostalCode <> Account.ShippingPostalCode
)


## Roll-Up Summary Fields
Roll-up summary fields calculate values from related child records.

Example completed:
Potential Value field on Account object that sums Expected Revenue from related Opportunities.


## College Admission Data Model
Using the same College Admission example:

### Objects
- College (Account)
- Student (Contact)
- Admission Application (Opportunity)
- Payment
- Department

### Relationships
- One College can have many Students
- One Student can have many Applications
- Applications can be linked to Departments

### Diagram
College
   │
   ├── Students
   │
   ├── Departments
   │
Students ─── Admission Applications

## Trailhead Modules Completed
- Data Modeling
- Formulas and Validations


## Reflection
Today I learned how Salesforce stores and connects business data using objects, fields, and relationships. I also learned how formulas, roll-up summary fields, and validation rules help automate logic and maintain accurate data.


## Screenshots
1. Data Modeling
<img width="477" height="780" alt="Screenshot 2026-05-16 210431" src="https://github.com/user-attachments/assets/34373fb2-233e-47a5-8ec5-3d0641cc531f" />

2. Formulas and Validations
<img width="611" height="805" alt="Screenshot 2026-05-16 213655" src="https://github.com/user-attachments/assets/b88a27aa-742c-4aae-b2c0-aaac8e53de43" />

