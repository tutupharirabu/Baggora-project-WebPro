# Baggora - Online Thrift Store

## Project Overview
Baggora is an online thrift store platform built with Laravel, targeting students around campus areas. The platform provides a marketplace for second-hand items with an emphasis on quality and affordability.

## Features
- **User Authentication**: Complete login and registration system
- **Product Catalog**: Browse products organized by categories with pagination
- **Product Details**: View detailed information about each product
- **Shopping Cart**: Add products to cart and manage shopping items
- **User Profile**: Update profile information and manage account settings
- **Newsletter Subscription**: Subscribe to newsletter for promotions and updates
- **Contact System**: Send messages to the Baggora team
- **Responsive Design**: Mobile-friendly UI built with Bootstrap 5

## Tech Stack
- **Backend**: PHP 8.x, Laravel Framework
- **Frontend**: HTML, CSS, JavaScript, Bootstrap 5
- **Database**: MySQL
- **Dependencies**: jQuery, Font Awesome, Bootstrap Icons

## Installation

### Prerequisites
- PHP >= 8.0
- Composer
- MySQL
- Node.js & NPM

### Steps
1. Clone the repository
```bash
git clone https://github.com/your-username/baggora.git
cd baggora
```

2. Install PHP dependencies
```bash
composer install
```

3. Create environment file
```bash
cp .env.example .env
```

4. Generate application key
```bash
php artisan key:generate
```

5. Configure database in `.env` file
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=baggora
DB_USERNAME=root
DB_PASSWORD=
```

6. Run migrations
```bash
php artisan migrate
```

7. Start the development server
```bash
php artisan serve
```

## Application Structure

### Models
- `User`: User authentication and profile data
- `emailSubs`: Newsletter subscription data
- `pesanKami`: User messages and contact form data

### Controllers
- `LoginController`: Handles user authentication
- `RegisterController`: Manages user registration
- `ProfileController`: Manages user profile updates
- `NewsletterController`: Handles newsletter subscriptions
- `PesanKamiController`: Processes contact form submissions

### Views
The application includes views for:
- Home page
- Product listings (with pagination)
- Product details
- Shopping cart
- User profile page
- About page
- Contact page

## Routes
The application defines routes for:
- Home page (`/home`)
- Product listings (`/barang-1`, `/barang-2`, `/barang-3`)
- Product details (e.g., `/detailbarang-1`)
- User authentication (`/login`, `/register`, `/logout`)
- User profile (`/profile`, `/update-profile`, `/update-password`)
- Contact page (`/kontak`, `/kirim-pesan`)
- About page (`/tentang`)
- Shopping cart (`/keranjang`)

## Database Structure
The application uses several tables:
- `tb_user`: Stores user information
- `tb_emailsubscription`: Stores newsletter subscriptions
- `tb_pesan`: Stores messages from the contact form

## Credits
Developed by Kelompok 6 - IT4501 - Web Programming:
- Irfan Zharauri Nanda Sudiyanto
- Hafiz Yazid
- Muhammad Rafi
- Fransiskus Ishak
