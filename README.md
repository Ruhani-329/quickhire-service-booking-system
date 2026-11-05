# QuickHire — Service Provider Booking & Management System

**A database-driven web application for discovering, booking, and managing local service providers.**

QuickHire is an academic Database Management System (DBMS) project developed using PHP and MySQL. The platform connects customers with service providers and supports service discovery, bookings, profile management, reviews, messaging, and administrative operations.

## Project Overview

Finding reliable service providers and managing appointments can be difficult when information is scattered across multiple channels.

QuickHire explores a centralized solution where customers can search for service providers, submit bookings, communicate with providers, and manage their service history.

The project emphasizes relational database design, backend development, and integration between user interfaces and persistent data.

## Key Features

### Customer Features
- User registration and login
- Browse and search for service providers
- View provider information and profiles
- Book services and review previous bookings
- Submit ratings and reviews
- Exchange messages with service providers
- Manage personal profile information

### Service Provider Features
- Provider registration and login
- Manage provider profile and service details
- View and manage customer bookings
- Update booking status
- Access subscription-related functionality

### Administrative Features
- Separate administrator login
- Administrative dashboard
- Management and monitoring functionality

## Technology Stack

| Component | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | PHP |
| Database | MySQL |
| Development Environment | XAMPP |
| Database Connectivity | PHP MySQLi |
| Version Control | Git and GitHub |

## Database Design

The application uses a relational MySQL database named `QUICKHIRE`.

The supplied SQL schema defines tables for the following entities:

| Table | Purpose |
|---|---|
| `users` | Customer account information |
| `provider` | Service provider profiles |
| `booking` | Service bookings and their status |
| `review` | Customer ratings and feedback |
| `messages` | User-to-user communication records |
| `saved_posts` | Saved provider references |
| `payment` | Booking-related payment records |
| `subscriptions` | Provider subscription records |
| `admin` | Administrator accounts |

### Database Concepts

- Relational database modeling
- Primary and foreign keys
- One-to-many relationships
- Composite primary keys
- Data integrity constraints
- SQL-based data storage and retrieval
- Database integration with PHP

## Application Workflow

1. A customer registers or logs into the platform.
2. The customer searches for a suitable service provider.
3. The customer views provider details and submits a booking.
4. The provider manages the booking through the application.
5. The customer can access booking history, messaging, and review functionality.
6. Administrators use a separate dashboard for administrative operations.

## Getting Started

### Prerequisites

- XAMPP with Apache and MySQL/MariaDB
- Web browser
- Git (optional)
- A code editor such as Visual Studio Code

### 1. Clone the Repository

```bash
git clone https://github.com/Ruhani-329/DBMS-project.git
```

Move the cloned project folder into the XAMPP `htdocs` directory.

### 2. Set Up the Database

1. Start Apache and MySQL from the XAMPP Control Panel.
2. Open `http://localhost/phpmyadmin`.
3. Create a database named `quickhire`.
4. Review and import the SQL definitions from `database_QuickHire.txt`.

**Important:** The current SQL file requires a small cleanup before importing: it contains a repeated `subscriptions` table definition.

### 3. Configure Database Connection

Open `db_config.php` and configure the local database connection according to your XAMPP settings.

Use local development credentials only. Do not publish real passwords or production credentials.

### 4. Run the Application

Open the following URL in your browser:

```text
http://localhost/DBMS-project/
```

The application's `index.php` redirects to the welcome page.

## Selected Project Files

| File | Description |
|---|---|
| `index.php` | Application entry point |
| `welcome.html` | Welcome page |
| `db_config.php` | Database connection configuration |
| `user_registration.php` | Customer registration |
| `register_provider.php` | Service provider registration |
| `find.php` | Service provider search |
| `booking.php` | Booking functionality |
| `booking_details.php` | Booking details |
| `previous_bookings.php` | Booking history |
| `review.php` | Review functionality |
| `send_message.php` | Messaging functionality |
| `admin_dashboard.php` | Administrator dashboard |
| `database_QuickHire.txt` | Database schema |

## Screenshots

Screenshots of the application interface can be added here to demonstrate the main workflows.

Suggested screenshots:
- Homepage
- Service provider search
- Booking interface
- Provider dashboard or profile
- Administrator dashboard

## Project Scope

QuickHire was developed as an academic DBMS project to demonstrate how a relational database supports the functionality of a web-based service marketplace.

The repository is intended for educational and portfolio purposes. Production deployment would require additional security reviews, validation, testing, and configuration improvements.

## Future Improvements

- Improved authentication and access controls
- Stronger server-side input validation
- Enhanced mobile-responsive interface
- Search and filtering improvements
- More comprehensive booking and payment workflows
- Automated testing and deployment documentation

## Author

**Ruhani Alam**

GitHub: [Ruhani-329](https://github.com/Ruhani-329)

---

*Academic Project | Database Management System | PHP & MySQL*
