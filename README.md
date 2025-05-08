# Xie Yi DC326958 Individual Project

## Overview

This project includes two parts. 

Part A is the fourth Project (Project Walkthrough Example by Mr. Web Designer).

Part B includes 5 different practices by Dani Krossing.

This project was developed by Xie Yi DC326958 as part of the CISC3003 course.


## Setup and Installation

These instructions are for setting up the project on a local machine using XAMPP.

### Prerequisites

*   XAMPP
    * Install tutorial: https://www.youtube.com/watch?v=mXdpCRgR-xE
    * Install website: https://www.apachefriends.org/index.html
*   A web browser
*   PHP Mailer (for PartB/Practice5)
    * Already included in my project

### Steps

1.  **Start XAMPP:** Launch the XAMPP Control Panel and start the Apache and MySQL modules.
    *   **Note on MySQL Port:** The project is configured to use port `3307` for MySQL in `db_config.php`. Ensure your XAMPP MySQL is running on this port, or update `db_config.php` and `my.ini` (XAMPP MySQL config) if you use the default port `3306`.

2.  **Place Project Files:**
    *   Copy the entire `CISC3003IndividualPRoject` project folder into your XAMPP web root directory (usually `htdocs`).

3.  **Create and Populate Database:**
    *   Open your web browser and go to `http://localhost/phpmyadmin/`.
    *   Create a new specific database with `utf8mb4_unicode_ci` collation in every project.
        *  In `ShoppingCartSystem`, name it `shop_db`
        *  In `Practice1`, name it `ooplogin`
        *  In `Practice2`, name it `phpproject01`
        *  In `Practice3`, you use `ooplogin`. It's same as `Practice1`, so no new database is needed to create
        *  In `Practice4`, name it `myfirstdatabase`
        *  In `Practice5`, name it `loginsystem`
    *   Select each database and go to the "Import" tab.
    *   Choose all SQL dump files (.sql) under each project directory and import them into their corresponding databases.
        *   For example, choose the `shop_db.sql` file from the project folder (`ShoppingCartSystem`) and import it into `shop_db`. This will create the necessary tables for this specific project.

4.  **Configure Email (Optional for Full Functionality):**
    *   In Practice5, for email verification to work, configure PHP's mail function. Now Practice5's verification emails are sent from my personal Gmail address. To get emails sent from your own Gmial address, please change all my Gmial address (starting with sharpstone) in `reset-request.inc.php` into yours. Also replace my password with your Gmail 2FA password. I use my personal email for college assignment needs. I will be removing my personal email information after I finish the course, so please do not steal it.

5.  **Access the Application:**
    *   Open your web browser and navigate to:
        `http://localhost/CISC3003IndividualPRoject/path-to-the-project/`
    *   (If you use a different Apache port, e.g., 8080, use `http://localhost:8080/CISC3003IndividualPRoject/path-to-the-project/`)


This README provides a basic guide to understanding, installing, and running Xie Yi's CISC3003IndividualProject.
