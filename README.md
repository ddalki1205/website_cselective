# Registration System (Website)
  - This project was made for university requirements. It is a Registration System inspired by Minecraft's official website, made using PHP, HTML5, CSS, JS, and MySQL.
  
> [!WARNING]
> I made this project without prior knowledge to full stack web development.

## Functionalities
  - User can register using first name, last name, email, and password.
  - User cannot re-use registered emails.

## Setup Guide

### 1. Install and Start XAMPP
  - Open **XAMPP Control Panel**
  - Start the following services: Apache (web server) and MySQL (database server)

### 2. Project Location (htdocs)

After cloning this project, it must be placed inside the XAMPP `htdocs` directory:

```
C:\xampp\htdocs\
```
### 3. phpMyAdmin (MySQL Database Setup)

1. Open phpMyAdmin:

```
http://localhost/phpmyadmin
````

2. Create a database (Click **New**)
2. Enter any database name (e.g. `mydatabase`)
3. Click **Create**
4. Create tables using the SQL tab or interface


### 4. Run the Website

Open your browser and go to:

```
http://localhost/full-stack-project/
```

Or directly:

```
http://localhost/full-stack-project/index.php
```

If Apache uses a different port:

```
http://localhost:8080/full-stack-project/
```

## Common Issues & Fixes

### Apache won’t start

* Port 80 or 443 may be in use
* Fix:

  * XAMPP → Apache → Config → `httpd.conf`
  * Change:

    ```
    Listen 80 → Listen 8080
    ```
  * Access site using:

    ```
    http://localhost:8080/mywebsite/
    ```

### MySQL won’t start

* Port 3306 may be used by another service (e.g. MySQL Workbench)
* Stop the conflicting service or change port in XAMPP

### Page not found (404)

* Ensure project is inside `htdocs`
* Check folder name spelling
* Ensure `index.php` exists