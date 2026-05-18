# Day 5 - Apex Introduction

## What is Apex?
Apex is Salesforce’s programming language used to add custom business logic to applications. It is similar to Java and runs on the Salesforce cloud platform. Apex is used when clicks, flows, and configurations are not enough for complex business requirements.


## Difference Between Flow and Apex

### Flow
- No-code / low-code automation
- Easy to build using drag and drop
- Best for simple to medium automation
- Faster to create

### Apex
- Code-based automation
- Used for complex logic
- More flexible and powerful
- Requires programming knowledge


## Configuration vs Coding

### Configuration
Configuration means building solutions using point-and-click tools without writing code.

Examples:
- Validation Rules
- Formula Fields
- Flow Builder
- Object creation

### Coding
Coding means writing custom logic using Apex.

Examples:
- Triggers
- Complex business calculations
- External API integrations


## Real Examples Where Apex Is Needed

### 1. Complex Fee Calculation
If a college calculates fees based on scholarship, attendance, category, and optional courses, Flow may become difficult. Apex can handle this complex logic easily.

### 2. External Payment Gateway Integration
If fee payment must connect with Razorpay or another payment system, Apex is needed for API integration.

### 3. Advanced Eligibility Logic
If admission eligibility depends on multiple conditions like marks, reservation, entrance exam score, and document verification, Apex is better.


## Integrated College Management System Design

### CRM
Tracks complete student admission journey.

### Objects
- Student
- Faculty
- Course
- Department
- Admission Application

### Relationships
- One Department has many Courses
- One Student can have many Applications
- Faculty teaches Courses

### Validation
- Email cannot be blank
- Age must be valid
- Seats cannot exceed limit

### Flow
- Send admission confirmation email
- Fee reminder notifications
- Seat availability updates

### Apex
- Scholarship fee calculation
- Eligibility checking logic
- Payment gateway integration


## Pseudocode Examples

### Example 1
IF seats are full
THEN block registration

### Example 2
IF attendance < 75%
THEN notify student

### Example 3
IF fee payment successful
THEN generate student ID card


## Reflection
Enterprise systems become complex over time. Click-based tools are useful for simple automation, but advanced business logic, integrations, and custom requirements need programming. Apex provides flexibility, scalability, and control for building enterprise-level applications.


## Screenshots

1. Apex & .NET Basics
   
<img width="1648" height="702" alt="Screenshot 2026-05-18 122238" src="https://github.com/user-attachments/assets/2d486aee-a836-4af2-86b1-f26bf4332c69" />

2. Apex Basics & Database
   
<img width="447" height="680" alt="Screenshot 2026-05-18 125838" src="https://github.com/user-attachments/assets/77f63ac5-d719-4c1c-b038-ccdeedaf3a97" />
