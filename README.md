# SkillGate
# SkillGate

SkillGate is a peer-to-peer learning platform built with PHP (MVC), MySQL, and Bootstrap.

## Features
- User registration and login with secure password hashing
- MVC architecture for clean code organization
- Responsive Bootstrap UI

## Technologies
- PHP, MySQL, PDO
- Bootstrap 5
- Apache with mod_rewrite

## Setup

1. Place the project in your web server root (e.g., `htdocs/skillswap`).
2. Create the database and table:

```sql
CREATE DATABASE skillswap;
USE skillswap;

CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100) UNIQUE,
  password VARCHAR(255),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);


Update config/config.php with your DB credentials.

Ensure Apache mod_rewrite is enabled and .htaccess is present.

Access via http://localhost/skillswap/login.
