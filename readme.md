# EduConsultPro - Salesforce CRM for Educational Institutions

![Salesforce](https://img.shields.io/badge/Salesforce-00A1E0?style=for-the-badge&logo=Salesforce&logoColor=white)

## Overview

EduConsultPro is a comprehensive Salesforce CRM solution designed specifically for educational institutions to manage their student lifecycle, from initial inquiry through enrollment and ongoing support. The platform provides a centralized system for managing courses, consultants, student data, appointments, and communication.

### Key Features

- **Student Admission Management**
  - Automated application process
  - Course selection and registration
  - Automated email notifications
  - Student data management

- **Appointment Scheduling System**
  - Consultant booking system
  - Automated approval process
  - Email notifications
  - Calendar management

- **Case Management**
  - Immigration support
  - Visa application tracking
  - Student support tickets

- **Course Management**
  - Course catalog
  - Registration tracking
  - Student enrollment

## Technical Architecture

### Custom Objects
- Student
- Course
- Consultant
- Appointment
- Registration

### Object Relationships
- Appointment → Student (Lookup)
- Appointment → Consultant (Lookup)
- Registration → Student (Lookup)
- Registration → Course (Lookup)
- Student → Case (Lookup)

### Automation Components

#### Flows
1. **Student Admission Flow**
   - Student information collection
   - Course selection
   - Registration creation
   - Email notifications

2. **Appointment Booking Flow**
   - Student verification
   - Consultant selection
   - Appointment scheduling
   - Approval process initiation

3. **Combined Master Flow**
   - New/Existing student routing
   - Process selection
   - Unified interface

#### Approval Processes
- Appointment approval workflow
- Manager-based routing
- Email notifications for submissions/approvals/rejections

### Lightning Components
- Custom Lightning App: "EduConsultPro"
- Custom Home Page
- Optimized navigation with essential tabs

## Setup Instructions

1. **Object Creation**
   ```
   - Import Course object and data
   - Import Consultant object and data
   - Import Student object and data
   - Create relationship fields
   ```

2. **User Configuration**
   ```
   - Create users with Standard Platform User profile
   - Configure user hierarchies for approval processes
   ```

3. **Flow Deployment**
   ```
   - Deploy Student Admission Flow
   - Deploy Appointment Booking Flow
   - Deploy Combined Master Flow
   ```

4. **Lightning App Setup**
   ```
   - Deploy EduConsultPro Lightning App
   - Configure home page layouts
   - Assign user permissions
   ```

## Custom Settings

### Case Object Configuration
- **Type Field Values:**
  - Immigration
  - Visa Application

- **Status Field Values:**
  - Open
  - In-Progress
  - Closed

## Features in Detail

### Student Admission Process
1. Student fills out admission form
2. Course selection
3. Automatic registration creation
4. Email confirmation sent
5. Student record created in system

### Appointment Management
1. Student verification
2. Consultant availability check
3. Appointment scheduling
4. Manager approval process
5. Email notifications

## System Requirements

- Salesforce Enterprise Edition or higher
- System Administrator profile for initial setup
- Standard Platform User license for end users

## Author

**Karri Vamsi Krishna**  
Gayatri Vidya Parishad College of Engineering(A), Visakhapatnam  
Roll Number: 21131A05C6  
Email: 21131A05C6@gvpce.ac.in

## Contributing

If you'd like to contribute to this project, please:
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE.md file for details

## Acknowledgments

- Gayatri Vidya Parishad College of Engineering
- Salesforce Development Team
- Project Mentors and Guides

---
*Note: This README is part of an academic project demonstrating Salesforce CRM implementation for educational institutions.*
