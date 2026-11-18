# CareSmile Dental Clinic

A web system for a dental clinic, built with Laravel. It has a public website for the clinic and separate dashboards for each type of user.

> Work in progress. Accounts, login and the role dashboards are in place. Clinic features such as appointments are still to come.

## Features

- Public pages: home and About CareSmile (mission, why choose us, contact details)
- Register, log in, reset your password and verify your email (Laravel Breeze)
- Three roles, each with its own dashboard:
  - **Admin**: dashboard and patient list
  - **Dentist**: dentist dashboard
  - **Patient**: patient dashboard (the default for new accounts)
- Profile page to update your details, change your password or delete your account

## Built with

- Laravel 12 (PHP 8.2) with Laravel Breeze
- MySQL
- Blade, Bootstrap, Tailwind CSS and Alpine.js, built with Vite

## Get started

```bash
git clone https://github.com/adeebirfaan/caresmile-dental-system.git
cd caresmile-dental-system
composer install
npm install
cp .env.example .env      # then set your database details
php artisan key:generate
php artisan migrate
npm run dev               # in one terminal
php artisan serve         # in another, then open http://localhost:8000
```

New accounts are patients. To make an admin or dentist, change the `role` column of that user in the `users` table to `admin` or `dentist`.
