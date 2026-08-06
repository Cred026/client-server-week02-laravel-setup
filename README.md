# client-server-week02-laravel-setup

---

Laravel is a modern PHP framework that simplifies web application development by providing built-in features to make development easier.

Client-server technology enables communication between users (clients) and web applications (servers), allowing data to be processed, stored, and retrieved efficiently.

The purpose of this project is to set up a Laravel development environment by installing PHP, Composer, Laravel, MariaDB/MySQL, and Git, then verifying the installation by running the default Laravel homepage using the Artisan development server.

---

The objectives that have been achieved in this project are;
Installing the required softwares
Configuring php.ini
Installing the basic laravel set up
Running the laravel project
Modifying the laravel Project

---

Operating System: Arch Linux
PHP Version: 8.5.9
Laravel Version: 5.31.1
Composer Version: 2.10.2
Git Version: 2.55.0
MariaDB Version: 12.3.2-MariaDB, client 15.2 for Linux (x86_64) using readline 5.1
VS Code Version: 1.131.0

---

## Installation Setup

### 1. Install PHP

Install PHP 8.2 or later and verify the installation:

```bash
php -v
```

### 2. Install Composer

Download and install Composer, then verify:

```bash
composer --version
```

### 3. Install Laravel

Install the Laravel installer:

```bash
composer global require laravel/installer
```

Or create a new project directly:

```bash
composer create-project laravel/laravel my-project
```

### 4. Install MariaDB/MySQL

Install MariaDB or MySQL, start the database service, and create a database for your Laravel project.

### 5. Install Git

Install Git and verify:

```bash
git --version
```

### 6. Run the Laravel Application

Navigate to the project directory and start the development server:

```bash
cd my-project
php artisan serve
```

Open the displayed local URL (typically `http://127.0.0.1:8000`) in your browser.

---

## Project Structure

- **app/** – Contains the core application logic, including controllers, models, middleware, and other classes.
- **routes/** – Defines the application's routes, such as web and API endpoints.
- **resources/** – Stores views (Blade templates), frontend assets, and language files.
- **public/** – Contains publicly accessible files, including the entry point (`index.php`) and assets like CSS, JavaScript, and images.
- **config/** – Holds configuration files for the application and its services.
- **database/** – Contains database migrations, seeders, and factories used for database management and testing.

---

'Laravel new project_name' not working because i have not configured php.ini to unconmment **inconv**

---

Throughout this activity, I learned how to set up a Laravel development environment by installing and configuring PHP, Composer, Laravel, MariaDB/MySQL, and Git. I also learned how these tools work together to support the development of modern web applications. After completing the installation, I successfully ran the default Laravel homepage using the Artisan development server, which helped me understand the basic workflow of a Laravel project.

The main challenge I encountered was during the installation process. Composer reported an error because the **iconv** PHP extension was not enabled. I initially forgot to modify the `php.ini` file and uncomment the required extension. After identifying the issue, I updated the configuration, enabled the extension, and restarted PHP. This resolved the problem and allowed Composer and Laravel to function correctly. This experience taught me the importance of checking PHP configuration files when troubleshooting installation errors.

Laravel is important in client-server development because it provides a structured and efficient framework for building web applications. It simplifies common tasks such as routing, database management, authentication, and request handling. By following the Model-View-Controller (MVC) architecture, Laravel helps developers write organized, maintainable, and scalable code, making it easier to build reliable client-server applications.

The knowledge I gained from this activity will help me in future software development projects by giving me confidence in setting up development environments and resolving configuration issues. It also introduced me to Laravel's development workflow, which will make it easier to build dynamic, database-driven web applications. Overall, this activity provided a solid foundation for learning Laravel and strengthened my understanding of client-server web development.

---

