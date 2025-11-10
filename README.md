# 🎓 Grading System (PHP + MySQL)

A **web-based Grading System** built with PHP and MySQL. Manage students, subjects, and grades — running locally using XAMPP.

---

## 🧰 Requirements

* **XAMPP** (Apache + PHP + MySQL)
* **Browser** (Chrome, Firefox, etc.)
* Optional: **Git** to clone instead of downloading ZIP

---

## 📥 Setup Instructions

### 1️⃣ Download or Clone the Project

**Option 1 — ZIP:**

* Click Code → Download ZIP
* Extract the folder

**Option 2 — Git:**

```bash
git clone https://github.com/PatrickJohnFajardo/Grading-System.git
```

* Move the folder to `C:\xampp\htdocs\GradingSystem`

### 2️⃣ Start XAMPP

* Open XAMPP Control Panel
* Start **Apache** and **MySQL**

### 3️⃣ Import the Database

* Go to `http://localhost/phpmyadmin/`
* Click **Databases** → Create database → name it `grading_system`
* Open it → Import → Choose File → select `database/schema.sql`
* Click **Go**

### 4️⃣ Configure the Connection

* Open `config/db.php`
* Set these values:

```php
$DB_HOST = 'localhost';
$DB_NAME = 'grading_system';
$DB_USER = 'root';
$DB_PASS = '';
```

* Save the file

### 5️⃣ Run the App

* Open browser → `http://localhost/GradingSystem/`

---

## 🔐 Default Logins

**Admin:**

* Username: `admin`
* Password: `Admin123!`

**Students:**

* Password: `Student123!`

---

## 📂 Folder Overview

| Folder   | Purpose                       |
| -------- | ----------------------------- |
| admin    | Admin dashboard, login/logout |
| students | Manage students & profiles    |
| subjects | Manage subject info           |
| includes | Shared header/footer files    |
| config   | DB & auth setup               |
| assets   | CSS & JS files                |
| database | SQL schema file               |
| uploads  | File uploads folder           |

**UI & Scripts:**

* `assets/custom.css` – Styles (maroon, yellow, white theme)
* `assets/custom.js` – JS features (form validation, alerts, grade calculator, CSV export)

---

## ⚠️ Common Issues

**Blank page or error?**

```php
ini_set('display_errors', 1);
error_reporting(E_ALL);
```

**Can’t log in?**

* Re-import `schema.sql` and use default credentials

**Apache won’t start?**

* Something’s using port 80. Stop Skype/IIS or change Apache port in XAMPP config

---

## 👨‍💻 Credits

Made by **Patrick John Fajardo**

* For educational and local testing purposes.
