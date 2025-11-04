# Sistema de Eventos

## Overview

Event management application that provides a simple interface to create, list, and manage events and user registrations. The project was built as an educational example and includes migrations, models, routes, and basic front-end assets to get a working application quickly.

This repository contains the full Laravel application in the `laravelproj/` folder.

## Key Features

- Create, edit and delete events
- Upload event images
- User authentication and event-user relations
- Database migrations and seeders included
- Basic responsive frontend (Tailwind + Vite)

## Tech Stack

- PHP (Laravel framework)
- MySQL (or compatible relational database)
- Composer for PHP dependencies
- Node.js, npm (Vite + Tailwind for front-end build)

## Requirements

- PHP 8.x (check `composer.json` for exact constraints)
- Composer
- Node.js 14+ and npm
- A database (MySQL, MariaDB, or SQLite for quick testing)

## Quick Start (Windows PowerShell)

1. Copy the example environment and configure your settings:

```powershell
cd "c:\Users\du-di\OneDrive\Área de Trabalho\laravel project\SistemaDeEventos-Laravel\laravelproj"
copy .env.example .env
```

2. Install PHP and Node dependencies:

```powershell
composer install
npm install
```

3. Generate the application key:

```powershell
php artisan key:generate
```

4. Create storage symlink (for uploaded files):

```powershell
php artisan storage:link
```

5. Run database migrations (and seed if needed):

```powershell
php artisan migrate
# Optional: php artisan db:seed
```

6. Start the development server (option A — Laravel built-in):

```powershell
php artisan serve
# Visit http://127.0.0.1:8000
```

Or (option B — using Vite for front-end hot reload):

```powershell
npm run dev
# Then open the app URL printed by the server or use php artisan serve in parallel
```

## Running Tests

The project includes PHPUnit configuration. Run tests with:

```powershell
php artisan test
# or: ./vendor/bin/phpunit
```

## Project Structure (high level)

- `app/` — application code (Models, Controllers, Providers)
- `config/` — Laravel configuration files
- `database/` — migrations, factories and seeders
- `public/` — web entry (assets, index.php)
- `resources/` — views, front-end assets, and Tailwind/Vite sources
- `routes/` — route definitions (`web.php`, `api.php`)

## Notes & Assumptions

- The main Laravel app is inside the `laravelproj/` directory.
- Update `.env` with your database credentials before running migrations.
- If using a remote storage (S3, etc.), configure `FILESYSTEM_DRIVER` in `.env`.

## Credits

This project was implemented following an educational course and adapted by the repository owner: [https://www.youtube.com/watch?v=4OxYHiEkqBg&amp;list=PLnDvRpP8BnewYKI1n2chQrrR4EYiJKbUG&amp;index=2](https://www.youtube.com/watch?v=4OxYHiEkqBg&list=PLnDvRpP8BnewYKI1n2chQrrR4EYiJKbUG&index=2)
