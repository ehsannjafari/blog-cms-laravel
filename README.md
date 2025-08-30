# 📘 Blog CMS (Laravel)

A multi-user blogging platform built with **Laravel 10**, **Tailwind CSS**, and **MySQL**.  
This project demonstrates core Laravel skills: authentication, roles/permissions, CRUD operations, image uploads, REST API, Docker, and testing.  

---

## 🚀 Features
- 🔐 User authentication (register, login, logout) using Laravel Breeze  
- 👥 Role-based access (Admin, Author, Reader)  
- 📝 Manage blog posts (create, edit, delete, publish/unpublish)  
- 🏷️ Categories & tags for posts  
- 🖼️ Image uploads with [Spatie Media Library](https://spatie.be/docs/laravel-medialibrary)  
- 🎨 Responsive UI with Tailwind CSS  
- 📡 REST API endpoints for posts & categories  
- 🧪 Unit & feature tests with PestPHP  
- 🐳 Dockerized setup for local development  
- 📊 Admin dashboard for managing users, posts, and categories  

---

## 🛠️ Tech Stack
- **Backend:** Laravel 10 (PHP 8+)  
- **Frontend:** Blade, Tailwind CSS, Alpine.js  
- **Database:** MySQL / PostgreSQL  
- **Authentication:** Laravel Breeze  
- **File Uploads:** Spatie Media Library  
- **Testing:** PestPHP  
- **DevOps:** Docker, Laravel Sail  

---

## 📂 Database Schema
**Users**  
- id, name, email, password, role (admin/author/reader)  

**Posts**  
- id, user_id, title, slug, content, status (draft/published), published_at  

**Categories**  
- id, name, slug  

**Tags**  
- id, name, slug  

**Post_Tag (Pivot)**  
- post_id, tag_id  

---

## 📂 Installation

### 1️⃣ Clone Repository
```bash
git clone https://github.com/YOUR_USERNAME/blog-cms-laravel.git
cd blog-cms-laravel
 ```
### 2️⃣ Install Dependencies
```bash
composer install
npm install && npm run dev
 ```
### 3️⃣ Configure Environment
```bash
cp .env.example .env
php artisan key:generate
 ```
###  Set up DB in .env
```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=blog_cms
DB_USERNAME=root
DB_PASSWORD=
 ```
### 4️⃣ Run Migrations & Seed Data
```bash
php artisan migrate --seed
 ```
### 5️⃣ Start Local Server
```bash
php artisan serve

 ```
