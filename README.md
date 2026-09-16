# Online Voting System

An online voting system for managing elections, voter registration, ballot casting, and result reporting in a secure and reliable way.

## Overview

This project is designed to support:

- Voter authentication and authorization
- Election creation and management
- Candidate and ballot setup
- Secure vote casting
- Result aggregation and reporting
- Audit logging for transparency and accountability

## Architecture

The system follows a modular client-server architecture with separate layers for:

- Client applications
- Security and access control
- Business services
- Data storage and auditing

A visual architecture diagram is available here:

- [online-voting-architecture.svg](online-voting-architecture.svg)

## Features

### For Voters
- Secure login
- View eligible elections
- Cast a vote only once per allowed election
- Receive confirmation after voting

### For Admins
- Create and manage elections
- Add candidates and ballot options
- Monitor voting status
- Publish election results

### For System Operators
- Audit logs and activity tracking
- High availability support
- Role-based access control
- Security monitoring and rate limiting

## Easy Tech Stack

This version uses a simple and beginner-friendly stack:

- Frontend: HTML, CSS, JavaScript
- Backend: Python (Flask)
- Database: SQLite
- Authentication: No authentication
- Styling: Bootstrap
- Deployment: Local server or simple hosting

This stack is easy to understand, lightweight, and suitable for a college or student project.

## Project Structure

```text
online-voting-system/
├── README.md
├── online-voting-architecture.svg
├── app/
│   ├── __init__.py
│   ├── models.py
│   ├── routes.py
│   ├── database.py
│   └── templates/
├── static/
│   ├── css/
│   └── js/
├── instance/
│   └── voting.db
├── requirements.txt
└── run.py
```

## Getting Started

1. Clone the repository.
2. Create a virtual environment.
3. Install dependencies from `requirements.txt`.
4. Set up SQLite database.
5. Run the Flask server.
6. Open the app in the browser and test election and voting flows.

### Example setup

```bash
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
python run.py
```

## Security Considerations

- Prevent duplicate voting
- Validate all form inputs on the server side
- Use SQLite safely with parameterized SQL queries
- Store vote records and admin actions in a simple audit trail
- Keep the app behind a local or restricted environment if used for demo purposes
- Add stronger security later if needed

## License

This project is for educational or demonstration purposes unless a separate license is added.

## Contributing

Contributions are welcome. Please keep changes focused, document major changes, and ensure that security requirements are preserved.
