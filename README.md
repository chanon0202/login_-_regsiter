# 🚀 PHP Login & Register System

[![PHP](https://img.shields.io/badge/PHP-8.2-blue?logo=php)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?logo=mysql)](https://www.mysql.com/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

This is a simple **Login and Register System** built with **PHP** and **MySQL (phpMyAdmin)**.  
It's perfect for beginners who want to learn basic user authentication systems.

---

## 🌟 Features
- ✅ User Registration with Username/Email duplication check
- ✅ User Login with Username and Password
- ✅ Passwords are securely **hashed** using `password_hash()`
- ✅ Logout functionality
- ✅ Dashboard accessible only to logged-in users

---

## 🛠 Technologies
- PHP
- MySQL (phpMyAdmin)
- HTML / CSS (can be customized with Tailwind or Bootstrap)

---

## 💾 Installation
1. Download this project to your local machine
2. Open **XAMPP / LAMP** and create a database named `my_website`
3. Create the `users` table using the following SQL:

```sql
CREATE TABLE users (
    id INT(11) AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL UNIQUE,
    email VARCHAR(100) NOT NULL UNIQUE,
    password VARCHAR(255) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
