# Day 6 - SOQL and Apex Triggers

## What is SOQL?
SOQL (Salesforce Object Query Language) is used to retrieve records from Salesforce objects. It is similar to SQL but specifically designed for Salesforce data. Developers use SOQL to query standard and custom objects, fetch related records, and filter data based on conditions.


## What is an Apex Trigger?
An Apex Trigger is a piece of code that runs automatically before or after specific events happen in Salesforce records, such as insert, update, delete, or undelete. Triggers help automate actions based on data changes.


## Flow vs Trigger

### Flow
- No-code / low-code automation
- Easy to build with drag-and-drop
- Best for simple automation
- Faster to create and maintain

### Apex Trigger
- Code-based automation
- Used for complex business logic
- Better for performance-heavy operations
- More flexible and scalable


## Before Trigger vs After Trigger

### Before Trigger
- Runs before records are saved
- Used for validation or modifying field values
- Faster because no extra DML needed

Example:
Set shipping address before saving account.

### After Trigger
- Runs after records are saved
- Used when record ID is required
- Used to create/update related records

Example:
Create follow-up task after opportunity closes.


## 5 Trigger Use Cases (College Management System)

1. After student registration → Send welcome email
Event: New student record created

2. After course becomes full → Notify faculty
Event: Course seat count reaches maximum

3. After attendance drops below 75% → Send warning
Event: Attendance record updated

4. After fee payment success → Generate payment confirmation
Event: Payment record updated

5. After admission approval → Create student portal login
Event: Application status changes to approved


## Query Examples (English Thinking)

- Find all students in Computer Science course
- Find all courses handled by Faculty Ravi
- Find students with attendance below 75%
- Find students who have not paid fees
- Find all approved admission applications


## Reflection
Enterprise systems need event-driven behavior because business actions must happen automatically when data changes. Manual monitoring is slow, error-prone, and inefficient. Automation improves speed, consistency, and user experience in large systems.


## Screenshots
- Database & .NET Basics badge

<img width="533" height="717" alt="Screenshot 2026-05-18 135220" src="https://github.com/user-attachments/assets/75502f02-fb3d-4b76-87a0-d7b161112810" />

- Apex Triggers badge

  <img width="462" height="722" alt="Screenshot 2026-05-18 144257" src="https://github.com/user-attachments/assets/76cbc669-2d69-4bf6-bce9-3b33389800ee" />
