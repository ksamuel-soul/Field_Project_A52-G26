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

# 📘 Database Schema Documentation

## 📂 Database Name: `field_project_batch_17`

## 📄 Table Name: `rider`

This table contains ride booking details including user information, travel source and destination, timing, vehicle details, pricing, and status-related fields.

---

### 🔢 Table Structure

| Column Name   | Data Type      | Description                                 | Constraints                         |
|---------------|----------------|---------------------------------------------|-------------------------------------|
| `R_id`        | INT            | Unique ID for each ride                     | Primary Key, Auto Increment, NOT NULL |
| `Username`    | VARCHAR(100)   | Name of the user requesting the ride        | NOT NULL                            |
| `Source`      | VARCHAR(100)   | Ride starting point                         | NOT NULL                            |
| `Destination` | VARCHAR(100)   | Ride ending point                           | NOT NULL                            |
| `Date`        | VARCHAR(20)    | Ride date                                   | NOT NULL                            |
| `Time`        | VARCHAR(20)    | Ride time                                   | NOT NULL                            |
| `Vehicle_Name`| VARCHAR(100)   | Name of the vehicle                         | NOT NULL                            |
| `Car_Num`     | VARCHAR(100)   | Vehicle registration number                 | NOT NULL                            |
| `Seat_Status` | INT            | Number of available seats                   | NULLABLE                            |
| `Price`       | BIGINT         | Fare price                                  | NULLABLE                            |
| `S_Username`  | VARCHAR(50)    | Username of the service provider (driver)   | NULLABLE                            |
| `Status`      | VARCHAR(50)    | Ride status                                 | Default: `Not_Booked`, NULLABLE     |
| `Pay_Status`  | VARCHAR(50)    | Payment status                              | NULLABLE                            |
| `Pay_Mode`    | VARCHAR(50)    | Mode of payment                             | NULLABLE                            |
| `Request`     | VARCHAR(50)    | Request status                              | NULLABLE                            |

---

