# 🏋️‍♂️ Fitness Training Portal

A full-featured fitness training platform built using **Angular**, **PHP (Laravel)**, and **MySQL**. Users can register, follow custom workout programs, track fitness progress, and follow personalized nutrition plans. Trainers can create and manage training content, while admins oversee the platform.

---

## 📌 Features

### 👤 General
- JWT Authentication (Login/Register)
- Role-based Access (Admin, Trainer, User)
- Mobile-responsive frontend (Angular + Material)
- In-app notifications and email support

### 🧑‍💪 Users (Trainees)
- Browse and enroll in workout programs
- Track daily workouts (reps, sets, weight)
- Access personalized nutrition/diet plans
- Progress dashboard and achievements

### 👨‍🏫 Trainers
- Create workout programs with videos and schedules
- Assign nutrition plans to users
- Monitor user progress
- Respond to user questions

### 👨‍💼 Admin
- Manage users and roles
- Approve/Reject trainer programs
- View analytics and reports
- Content moderation tools

---

## 🛠️ Tech Stack

| Layer         | Technology                         |
|---------------|-------------------------------------|
| Frontend      | Angular 17 + Angular Material       |
| Backend       | PHP (Laravel 10)                    |
| Database      | MySQL                               |
| Auth          | JWT-based authentication            |
| Media Storage | Local (uploads/) or AWS S3          |
| Charts        | Chart.js / ngx-charts               |

---

## 🚀 Getting Started

### 📦 Requirements
- Node.js (18+)
- PHP (8.1+)
- Composer
- MySQL (5.7 or 8.x)

### 🔧 Setup Instructions

#### 1. Clone the Repository
```bash
git clone https://github.com/your-username/fitness-training-portal.git
cd fitness-training-portal
```

#### 2. Setup the Angular Frontend
```bash
cd angular-frontend
npm install
ng serve
```
App will run at: [http://localhost:4200](http://localhost:4200)

#### 3. Setup the Laravel Backend
```bash
cd ../php-backend
composer install
cp .env.example .env
php artisan key:generate
```
Edit the `.env` file and update the following lines with your MySQL credentials:
```env
DB_DATABASE=fitness_portal
DB_USERNAME=root
DB_PASSWORD=your_password
```
Then run the migrations and seeders:
```bash
php artisan migrate --seed
php artisan serve
```
API will run at: [http://localhost:8000](http://localhost:8000)

#### 4. Database
MySQL setup using `database/schema.sql` and `seed.sql`

Make sure to match DB credentials in the `.env` file.

📜 License
MIT License. You are free to use, modify, and distribute.


---

Let me know if you want this tailored for **plain PHP** instead of Laravel, or if you’d like a **GitHub README badge setup** (CI, version, license, etc.) included!
