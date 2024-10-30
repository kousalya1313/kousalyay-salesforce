EduConsultPro - Salesforce CRM for Educational Institutions
Salesforce

Overview
EduConsultPro is a comprehensive Salesforce CRM solution tailored for educational institutions. It streamlines the entire student lifecycle, from initial inquiry and enrollment to ongoing support. This centralized platform manages courses, consultants, student data, appointments, and communication effectively.

Demonstration
![EduConsultPro Demo]

Watch the video above for a complete demonstration of EduConsultPro's features and functionality.

Key Features
Student Admission Management:

Automated application process
Course selection and registration
Automated email notifications
Comprehensive student data management
Appointment Scheduling:

Consultant booking system
Automated approval process
Timely email notifications
Integrated calendar management
Case Management:

Immigration support
Visa application tracking
Student support ticketing system
Course Management:

Comprehensive course catalog
Registration tracking
Student enrollment management
Technical Architecture
Custom Objects
Student
Course
Consultant
Appointment
Registration
Object Relationships
Appointment → Student (Lookup)
Appointment → Consultant (Lookup)
Registration → Student (Lookup)
Registration → Course (Lookup)
Student → Case (Lookup)
Automation
Flows:

Student Admission Flow: Handles student information collection, course selection, registration, and email notifications.
Appointment Booking Flow: Manages student verification, consultant selection, appointment scheduling, and approval initiation.
Combined Master Flow: Provides a unified interface, routing new/existing students and directing them to the appropriate process.
Approval Processes: Appointment approval workflow with manager-based routing and email notifications for submissions, approvals, and rejections.

Apex Triggers:

StudentTrigger: This trigger automatically creates a welcome case when a new student record is inserted. The case is used to track the student's onboarding process.
AppointmentTrigger: This trigger performs the following actions:
Before Insert/Update: Validates that appointments are scheduled during business hours (9 AM to 5 PM) and that the chosen consultant is available at the requested time.
After Insert: Sends email notifications to both the student and the consultant confirming the newly scheduled appointment.
User Interface
Lightning Components:
Custom Lightning App: "EduConsultPro"
Custom Home Page for optimized user experience
Streamlined navigation with essential tabs
Setup Instructions
Object Creation:

Import Course object and data.
Import Consultant object and data.
Import Student object and data.
Create necessary relationship fields between objects.
User Configuration:

Create users with the "Standard Platform User" profile.
Configure user hierarchies for approval processes.
Flow Deployment:

Deploy the Student Admission Flow.
Deploy the Appointment Booking Flow.
Deploy the Combined Master Flow.
Lightning App Setup:

Deploy the EduConsultPro Lightning App.
Configure home page layouts for optimal user experience.
Assign user permissions for app access.
Custom Settings
Case Object Configuration
Type Field Values: Immigration, Visa Application
Status Field Values: Open, In-Progress, Closed
Features in Detail
Student Admission Process
Student completes the admission form.
Student selects desired courses.
System automatically creates the registration record.
Confirmation email is sent to the student.
Student record is created in Salesforce.
Appointment Management
System verifies student information.
Consultant availability is checked.
Appointment is scheduled based on availability.
Appointment is submitted for manager approval.
Email notifications are sent throughout the process.
System Requirements
Salesforce Enterprise Edition or higher
System Administrator profile for initial setup
Standard Platform User license for end users
Author
YAVANAMANDA SRI PHANI KOUSALYA
Gayatri Vidya Parishad College of Engineering(W), Visakhapatnam
Roll Number: 21JG1A4263
Email: 21jg1a4263.kousalya@gvpcew.ac.in

License
This project is licensed under the MIT License - see the LICENSE.md file for details.

Acknowledgments
Gayatri Vidya Parishad College of Engineering For Women
Salesforce Development Team
Project Mentors and Guides
Note: This README is part of an academic project demonstrating Salesforce CRM implementation for educational institutions.
