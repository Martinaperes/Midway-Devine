
**MidwayCafe**:

---

````markdown
# ☕ MidwayCafe – Cafe Management System

MidwayCafe is a web-based cafe management system designed to streamline and modernize cafe operations. It allows users to register, log in, and make reservations seamlessly, while chefs can view incoming requests and manage their part efficiently.

Built with *Laravel* and *MySQL*, the application follows the *MVC (Model-View-Controller)* architecture pattern for clean and scalable code organization.

---

## ✨ Features

- ✅ User registration and login
- 🗓️ Reservation system for customers
- 👨‍🍳 Chef dashboard to view and manage orders
- 📦 Structured MVC architecture using Laravel
- 🔐 Secure authentication and data handling
- 📊 MySQL database for efficient storage

---

## 🛠 Tech Stack

| Layer       | Technology         |
|-------------|--------------------|
| Framework   | Laravel (PHP)      |
| Backend     | PHP (Laravel MVC)  |
| Database    | MySQL              |
| Frontend    | Blade Templates    |
| Auth        | L Auth Scaffolding |
| Deployment  | In Cpanel          |

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Martinaperes/Midway-Devine.git
cd Midway-Devine
````

### 2. Install Dependencies

```bash
composer install
```

### 3. Setup Environment File

```bash
cp .env.example .env
php artisan key:generate
```

Update `.env` with your MySQL database credentials:

```
DB_DATABASE=your_db_name
DB_USERNAME=your_db_user
DB_PASSWORD=your_db_password
```

### 4. Run Migrations

```bash
php artisan migrate
```

### 5. Serve the Application

```bash
php artisan serve
```

The app will be running at `http://localhost:8000`.

---

## 👨‍💻 Authors

* **Dennis Muuo**
* **Martina Peres**

We collaborated to bring this idea to life, blending backend functionality with a simple user interface, all while learning and applying real-world Laravel development practices.

---

## 🏁 Project Structure (MVC)

```
app/
  ├── Http/
  │   ├── Controllers/    # Handles app logic
  ├── Models/             # Eloquent models
resources/
  ├── views/              # Blade templates (HTML UI)
routes/
  └── web.php             # Route definitions
database/
  ├── migrations/         # Database tables
```

---

## 📌 Purpose

MidwayCafe was built to help local cafes:

* Manage reservations with ease
* Provide chefs with a clear queue of customer requests
* Reduce manual operations and paperwork
* Improve customer experience through online accessibility

---

## 📄 License

This project is licensed for personal or educational use. For any commercial use or contributions, please contact the authors.

dennis: dennismuuo.dev@gmail.com
martina: 1martinaperes@gmail.com

---

## Contribution

Pull requests and issues are welcome! Let’s improve the cafe experience together.

```
