# EduConsultPro - Educational Consultation Management System

A Flask-based web application integrated with Salesforce CRM to manage educational consultation services.

## Features

- Student registration and management
- Course enrollment
- Appointment scheduling with consultants
- Support case management
- Integration with Salesforce CRM

## Prerequisites

- Python 3.7+
- Salesforce Developer Account
- Flask and required packages

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd eduConsultPro
```

2. Create a virtual environment and activate it:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

4. Set up your environment variables:
- Copy `.env.example` to `.env`
- Fill in your Salesforce credentials and Flask secret key

5. Initialize the database:
```bash
flask db upgrade
```

## Salesforce Setup

1. Create the following custom objects in Salesforce:
   - Student__c
   - Course__c
   - Consultant__c
   - Appointment__c
   - Registration__c

2. Configure custom fields as per the application requirements

3. Set up approval processes for appointments

## Running the Application

1. Ensure your virtual environment is activated
2. Run the Flask application:
```bash
flask run
```

3. Access the application at `http://localhost:5000`

## Project Structure

```
eduConsultPro/
├── app/
│   ├── __init__.py
│   ├── routes.py
│   ├── models.py
│   └── templates/
│       ├── base.html
│       ├── home.html
│       ├── login.html
│       ├── register.html
│       ├── dashboard.html
│       ├── book_appointment.html
│       └── create_case.html
├── .env
├── config.py
├── requirements.txt
└── README.md
```

## Security Considerations

- Ensure proper authentication and authorization
- Protect sensitive credentials
- Use HTTPS in production
- Implement rate limiting
- Regular security updates

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
