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
php artisan make:seeder DatabaseSeeder 
//ads user roles (crucial) and two example database users: regular user: user password123; admin: admin password123

after starting apache in xammp, main page should be available at:
http://localhost/public_html/RealEstateApp/public/

