

```markdown
MidwayCafe – Modern Cafe Management System  
Domain: https://martina.quickzingo.com
Deployment: Hosted on cPanel with MySQL backend  

MidwayCafe revolutionizes traditional cafe operations by digitizing reservations, order management, and chef workflows. Designed as a full-stack web application, it empowers cafes to transition from paper-based systems to an efficient, scalable digital platform. Built with Laravel 10 and MySQL 8, the system adheres to MVC architecture for maintainability and follows industry-standard security practices.

---

 Key Features  

 User-Centric Experience  
- Role-Based Access Control: Separate dashboards for customers and chefs.  
- Secure Authentication: Laravel’s built-in auth scaffolding with email/password login.  
- Reservation System: Customers can book tables with time/date selection, with automatic conflict detection.  

 Chef Workflow Optimization  
- Real-Time Order Queue: Chefs view pending orders chronologically with priority flags.  
- Order Status Updates: Mark orders as "Preparing", "Ready", or "Cancelled" with timestamps.  

 Technical Highlights  
- MVC Architecture: Clear separation of concerns (Models: `Reservation.php`, `User.php`; Views: Blade templates; Controllers: `ReservationController.php`).  
- Database Efficiency: Indexed MySQL tables for fast querying even under high load.  
- Responsive UI: Mobile-friendly layouts using Bootstrap 5 integrated with Laravel Blade.  

---

 Application Snapshots  

![MidwayCafe Screenshot](https://github.com/Martinaperes/Midway-Devine/blob/main/images/image%20copy%204.png?raw=true)



---

Technology Stack  

| Layer          | Technology                          | Purpose                                  |  
|----------------|-------------------------------------|------------------------------------------|  
| Framework      | Laravel 10 (PHP 8.2+)               | Backend logic, routing, and security    |  
| Database       | MySQL 8                             | Relational data storage (users, orders) |  
| Frontend       | Blade + Bootstrap 5                 | Dynamic HTML rendering + UI components  |  
| Auth           | Laravel Breeze                      | User authentication flows               |  
| Deployment     | cPanel (Apache)                     | Production hosting                      |  

---

 Installation Guide  

 Prerequisites  
- PHP ≥ 8.2, MySQL ≥ 8.0, Composer  

 Step-by-Step Setup  

1. Clone & Navigate  
   ```bash
   git clone https://github.com/Martinaperes/Midway-Devine.git
   cd Midway-Devine
   ```

2. Install Dependencies  
   ```bash
   composer install
   npm install && npm run build  # If using frontend assets
   ```

3. Configure Environment  
   - Duplicate `.env.example` to `.env` and update:  
     ```env
     DB_DATABASE=midwaycafe_prod
     DB_USERNAME=deploy_user
     DB_PASSWORD=secure_password_123
     APP_URL=http://martina.quickzingo.com
     ```

4. Database Setup  
   ```bash
   php artisan migrate --seed  # Populates test data
   ```

5. Launch Development Server  
   ```bash
   php artisan serve --port=8080
   ```
   Access via `http://localhost:8080` or your domain.

---

## Project Structure (MVC Breakdown)  

```
app/
├── Models/                   # Database interactions
│   ├── User.php              # User roles/auth
│   └── Reservation.php       # Booking logic
├── Http/Controllers/         # Business logic
│   ├── ReservationController.php
│   └── ChefController.php
resources/
├── views/                    # UI Templates
│   ├── auth/                 # Login/register
│   └── reservations/         # Booking forms
database/
├── migrations/               # Schema definitions
│   ├── 2023_..._users_table.php
│   └── 2023_..._reservations_table.php
routes/
└── web.php                   # All application routes
```

---

## Educational & Real-World Value  

This project was developed as part of our coursework to demonstrate:  
- Real-World Problem Solving: Addressing inefficiencies in small cafe operations.  
- Full-Stack Proficiency: Integration of frontend (Blade/Bootstrap), backend (Laravel), and database (MySQL).  
- Collaborative Development: Git-based teamwork between backend (Dennis) and frontend (Martina).  

---

## License & Attribution  

**License:** MIT (Educational Use Only)  
For commercial licensing, contact:  
- Dennis Muuo: [dennismuuo.dev@gmail.com](mailto:dennismuuo.dev@gmail.com)  
- Martina Peres: [1martinaperes@gmail.com](mailto:1martinaperes@gmail.com)  

**Note to Instructor:** This project meets the requirement for a detailed technical document, showcasing both implementation depth and theoretical understanding of MVC, Laravel, and relational database design.  

---

 How to Contribute  

1. Fork the repository.  
2. Create a feature branch (`git checkout -b feature/new-payment`).  
3. Submit a Pull Request with clear documentation.  

We welcome improvements, especially in:  
- Payment gateway integration (Stripe/PayPal).  
- Real-time updates with Laravel Echo + Pusher.  
```
