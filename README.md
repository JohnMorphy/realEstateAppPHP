# realEstateAppPHP
A basic real estate that allows registration, placing offers, browsing and basic admin panel.

Prerequisites
PHP: Ensure you have PHP installed. You can download it from php.net.
Composer: A dependency manager for PHP. Download and install it from getcomposer.org.
XAMPP: A free and open-source cross-platform web server solution stack package developed by Apache Friends. Download it from apachefriends.org.

How i ran it on a local apache server, with a local database:
Using xampp, place folder in public_html folder -> xampp\htdocs\public_html.

Connect to your postgres server (hosted locally or a virtual machine).
In app in main folder in .env file, adjust connection data accordingly (username and password, if locally hosted/using tunnel host should remain at localhost).

On postgres server create schema: laravel_realestateapp (or you can change its name in .env file).

Migrate database using artisan migration:
In the root of the project cmd command/integrated vs studio terminal:

composer install
php artisan key:generate
php artisan migrate
php artisan db:seed
//ads user roles (crucial) and two example database users: regular user: user@example.com password123; admin: admin@example.com password123

after starting apache in xammp, main page should be available at:
http://localhost/public_html/RealEstateApp/public/

// viewing offers
![image](https://github.com/JohnMorphy/realEstateAppPHP/assets/92916894/dda2a7bb-cd92-422d-9e24-daa7ecf5d8cf)
![image](https://github.com/JohnMorphy/realEstateAppPHP/assets/92916894/30fd3b88-5399-4303-abb6-d81c5b8fd590)

// adding offers - allows for uploading images
![image](https://github.com/JohnMorphy/realEstateAppPHP/assets/92916894/f4b5baaf-8f7f-491f-b354-b230ecce7fdd)

// editing offers & personal panel
![image](https://github.com/JohnMorphy/realEstateAppPHP/assets/92916894/aa589147-9767-4146-9284-6f64f8e6a95a)
![image](https://github.com/JohnMorphy/realEstateAppPHP/assets/92916894/a83301e4-f7a6-4194-8815-d540fdd0e28f)

// admin dashboard
![image](https://github.com/JohnMorphy/realEstateAppPHP/assets/92916894/b2f0bb44-c2a1-4bf5-9334-4802d424d9c4)
![image](https://github.com/JohnMorphy/realEstateAppPHP/assets/92916894/b3e23021-0077-407d-86ee-1fb71818fe98)

