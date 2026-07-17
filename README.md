# Warehouse Inventory Management System (WIMS)

A modern Warehouse Inventory Management System (WIMS) built with Laravel and React to streamline warehouse operations, inventory tracking, and logistics management. The application provides a centralized platform for managing products, warehouses, vendors, customers, inventory movements, inbound deliveries, outbound deliveries, and goods receipts. It is designed with a modular architecture to support scalable warehouse operations while maintaining an intuitive user experience.

---

## Overview

Warehouse Inventory Management System (WIMS) simplifies day-to-day warehouse activities by providing complete visibility into inventory movement from receiving goods to dispatching customer orders.

The application follows the Laravel MVC architecture with a React frontend powered by Inertia.js, allowing a modern single-page application experience while leveraging Laravel's robust backend ecosystem.

---

# Key Features

## Dashboard

- Centralized operational dashboard
- Quick access to warehouse modules
- Inventory overview
- Warehouse activity summary

---

## Authentication

- Secure user authentication
- Session-based login
- Password hashing
- Protected application routes

---

## User Management

- Manage application users
- Role-based access using Spatie Laravel Permission
- User profile management

---

## Product Management

- Create products
- Update product information
- Delete products
- Search products
- Product inventory tracking

---

## Warehouse Management

- Create warehouses
- Manage warehouse information
- Multiple warehouse support

---

## Location Management

- Define warehouse locations
- Organize inventory storage
- Structured warehouse layout

---

## Vendor Management

- Maintain supplier records
- Vendor information management
- Supplier lookup

---

## Customer Management

- Customer registration
- Customer information management
- Customer order references

---

## Inventory Management

- Real-time inventory tracking
- Inventory updates
- Stock visibility
- Inventory lookup

---

## Inbound Deliveries

Manage incoming shipments from vendors.

Features include:

- Create inbound deliveries
- Update delivery information
- Track receiving status

---

## Goods Receipt

Record received inventory into the warehouse.

Supports:

- Goods receipt creation
- Inventory updates
- Warehouse allocation

---

## Outbound Deliveries

Manage products leaving the warehouse.

Features include:

- Outbound shipment creation
- Dispatch tracking
- Inventory deduction

---

## Delivery Orders

Create and manage customer delivery orders.

Supports:

- Delivery order creation
- Order tracking
- Customer shipment management

---

## Authorization

Role and permission management powered by:

- Spatie Laravel Permission

---

## API Foundation

API controllers are included within the project structure for future API expansion.

---

# Tech Stack

| Category | Technologies |
|----------|--------------|
| **Backend** | Laravel 9, PHP 8 |
| **Frontend** | React, Inertia.js |
| **UI Framework** | Material UI (MUI), Tailwind CSS |
| **Styling** | Tailwind CSS, CSS3 |
| **State Management** | React Hooks, React Query |
| **Forms & Validation** | Formik |
| **Data Visualization** | Recharts |
| **Data Tables** | TanStack Table, MUI Data Grid |
| **Icons** | React Icons |
| **Authentication** | Laravel Breeze, Laravel Sanctum |
| **Authorization** | Spatie Laravel Permission |
| **Database** | MySQL / MariaDB |
| **ORM** | Laravel Eloquent ORM |
| **Routing** | Laravel Router, Ziggy |
| **API** | RESTful API (Laravel) |
| **Package Managers** | Composer, npm |
| **Build Tool** | Vite |
| **HTTP Client** | Guzzle HTTP |
| **Testing** | PHPUnit, Laravel Dusk |
| **Containerization** | Docker |
| **Version Control** | Git, GitHub |
| **Architecture** | MVC (Model-View-Controller) |
| **Development Tools** | Laravel Artisan, Tinker |
| **Deployment Ready** | Apache, Nginx, Docker |
| **Logging** | Laravel Log, Monolog |
| **Caching** | Laravel Cache |
| **Session Management** | Laravel Sessions |
| **Queue Support** | Laravel Queue (Database Driver Ready) |
| **File Storage** | Laravel Storage, Public Disk |
| **Configuration** | Environment-based Configuration (.env) |
| **Security** | CSRF Protection, Password Hashing, Middleware, Input Validation |

---

# Project Structure

```
app/
 ├── Http/
 ├── Models/
 ├── Providers/

bootstrap/

config/

database/
 ├── factories/
 ├── migrations/
 └── seeders/

public/

resources/
 ├── css/
 ├── js/

routes/
 ├── web.php
 ├── api.php
 └── auth.php

storage/

tests/
```

---

# Business Workflow

```
Vendor
      │
      ▼
Inbound Delivery
      │
      ▼
Goods Receipt
      │
      ▼
Warehouse Inventory
      │
      ▼
Customer Order
      │
      ▼
Outbound Delivery
      │
      ▼
Delivery Order
```

---

# Database Modules

The application is organized around several business entities:

- Users
- Products
- Warehouses
- Locations
- Vendors
- Customers
- Inventory
- Inbound Deliveries
- Goods Receipts
- Outbound Deliveries
- Delivery Orders

These modules work together to provide complete warehouse inventory tracking.

---

# Architecture

```
React Frontend
        │
        ▼
 Inertia.js
        │
        ▼
Laravel Controllers
        │
        ▼
 Eloquent Models
        │
        ▼
 Database
```

The project follows Laravel's MVC architecture, separating presentation, business logic, and data access while using React for a modern user interface.

---

# Installation

## Clone Repository

```bash
git clone https://github.com/your-username/warehouse-inventory-management-system.git

cd warehouse-inventory-management-system
```

## Install PHP Dependencies

```bash
composer install
```

## Install Node Packages

```bash
npm install
```

## Configure Environment

```bash
cp .env.example .env
```

Update database credentials inside the `.env` file.

---

## Generate Application Key

```bash
php artisan key:generate
```

---

## Run Database Migrations

```bash
php artisan migrate
```

If seeders are available:

```bash
php artisan db:seed
```

---

## Storage Link

```bash
php artisan storage:link
```

---

## Start Development Server

```bash
php artisan serve
```

---

## Start Vite

```bash
npm run dev
```

---

# Environment Variables

Typical Laravel configuration includes:

```env
APP_NAME=

APP_ENV=

APP_KEY=

APP_DEBUG=

APP_URL=

DB_CONNECTION=

DB_HOST=

DB_PORT=

DB_DATABASE=

DB_USERNAME=

DB_PASSWORD=

CACHE_DRIVER=

SESSION_DRIVER=

QUEUE_CONNECTION=

MAIL_MAILER=
```

---

# Security

The project includes standard Laravel security features including:

- Authentication
- Authorization
- Password hashing
- CSRF protection
- Input validation
- Route middleware
- Role & Permission management
- Sanctum integration

---

# Frontend

The frontend is developed using:

- React
- Inertia.js
- Material UI
- Tailwind CSS
- React Icons
- Formik
- TanStack Table
- Recharts

This combination provides a responsive and interactive user interface for warehouse management.

---

# Testing

Testing support includes:

- PHPUnit
- Laravel Dusk

Run tests using:

```bash
php artisan test
```

---

# Performance

Recommended production optimizations:

```bash
php artisan config:cache

php artisan route:cache

php artisan view:cache

php artisan optimize
```

---

# Deployment

The application can be deployed using:

- Apache
- Nginx
- Docker
- VPS
- Cloud Hosting

Before deployment:

- Configure production environment variables.
- Disable debug mode.
- Cache configuration and routes.
- Use HTTPS.
- Configure proper file permissions.

---

# Screenshots

Add screenshots of the following sections:

- Login
- Dashboard
- Products
- Warehouses
- Inventory
- Vendors
- Customers
- Goods Receipt
- Outbound Delivery
- Reports

Example:

```
docs/screenshots/dashboard.png

docs/screenshots/products.png

docs/screenshots/inventory.png
```

---

# Future Enhancements

Potential improvements include:

- REST API expansion
- Barcode support
- QR code scanning
- Inventory forecasting
- Email notifications
- Multi-language support
- Audit logs
- Purchase Orders
- Sales Orders
- Reports & Analytics
- Mobile application
- Dashboard widgets
- File attachments
- Activity logs
- Real-time notifications
- Background job processing
- Advanced search & filtering
- Inventory alerts
- Low stock notifications
- Import/Export functionality

---

# Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push to your branch.
5. Open a Pull Request.

---

# License

This project is licensed under the MIT License unless otherwise specified.

---

# Author

**Your Name**

GitHub: https://github.com/your-username

LinkedIn: https://linkedin.com/in/your-profile

Email: your-email@example.com

---

# Acknowledgements

Built with:

- Laravel
- React
- Inertia.js
- Material UI
- Tailwind CSS
- Vite
- Spatie Laravel Permission
- Laravel Sanctum

---

## Project Status

This project is actively developed as a modern Warehouse Inventory Management System, focusing on inventory control, warehouse operations, and logistics workflows using the Laravel ecosystem and a React-based frontend.
