Download the following packages:- 

Make sure you have Php installed in your system..!!!  

   The provided link is Php Version 8.4 
   *      https://windows.php.net/downloads/releases/php-8.4.8-nts-Win32-vs17-x64.zip

using composer download the below packages... 
*      https://getcomposer.org/Composer-Setup.exe

Using Composer:-     
1. PHPMailer:-
   
       composer require phpmailer/phpmailer
3. Google/apiclient:-  
      
       composer require google/apiclient
   
PhpMailer:-
*       https://github.com/PHPMailer/PHPMailer
Google/apiclient:-
*      https://packagist.org/packages/google/apiclient
Note:- Inside vendor folder make sure you have the autoload.php


# 📘 Database Schema Documentation

## 📂 Database Name: `field_project_batch_17`

## 📄 Table Name: `acc_registration`

This table stores account registration details including user personal information, login credentials, and a reference to an image source. It contains 7 columns.

---

### 🔢 Table Structure

| Column Name  | Data Type       | Description                           | Constraints                            |
|--------------|------------------|---------------------------------------|----------------------------------------|
| `S.No`       | INT              | Unique ID for each user               | Primary Key, Auto Increment, NOT NULL  |
| `First_Name` | VARCHAR(100)     | User's first name                     | NOT NULL                               |
| `Last_Name`  | VARCHAR(100)     | User's last name                      | NOT NULL                               |
| `Email`      | VARCHAR(100)     | User's email address                  | NOT NULL                               |
| `Phone_No`   | VARCHAR(100)     | User's phone number                   | NOT NULL                               |
| `Password`   | VARCHAR(50)      | User's password (hashed)              | NOT NULL                               |
| `img_src`    | VARCHAR(500)     | Path or URL to the user image source | NOT NULL                               |

---

### 🔐 Primary Key

- `S.No` is the **Primary Key** and is **Auto Incremented** to uniquely identify each record.

---

### 🌐 Collation

- All text fields use: `utf8mb4_0900_ai_ci` collation.

---

### 🗂️ Notes

- All fields are **mandatory** (no `NULL` values allowed).
- No default values are set.
- No partitioning is defined for the table.

